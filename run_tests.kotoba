(babashka.classpath/add-classpath "src:test")
(require '[clojure.test :as t])

(def suites
  '[kafun.methods.test-kafun-edn
    kafun.methods.test-remediate
    kafun.methods.test-kotoba
    kafun.methods.test-autorun
    kafun.methods.test-ie-flow
    kafun.methods.test-digest
    kafun.methods.test-bottleneck
    kafun.methods.test-dynamics
    kafun.methods.test-react-loop
    kafun.repository-contract-test])
(apply require suites)
(let [{:keys [fail error]} (apply t/run-tests suites)]
  (System/exit (if (zero? (+ fail error)) 0 1)))
