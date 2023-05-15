# Description of the policy

The ClusterPolicy specifies the following rule. If there is any ConfigMap resource in the *team-\** (regex) namespace, add the label **lfx-mentorship: kyverno**, 
if and only if the ConfigMap has no labels described in its metadata. 


## Description of the testsuite

This is a TestSuite created for the ClusterPolicy for ConfigMaps. The folder also contains **kuttl-test.yaml**
which helps in setting the testsuite configuration. Setting up the configuration helps us running the tests directly without the testsuite folder :-
 `kubectl kuttl test`


**The TestSuite consists of the following test scenarios:-**
1. test1(HasNoLabels)
2. test2(HasLabels)
3. test3(DifferentNameSpace)


