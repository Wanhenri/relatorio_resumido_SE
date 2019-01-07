# relatorio_resumido_SE
Destinado para acrescentar pontos interessantes para o mestrado em SE

---

#### text: Claims about the use of software engineering practices in science: a systematic literature review

<p>LM1: Scientific software developers generally do not use a for-mal software development methodology.
We identified nine stud-ies that made this claim[2,3,16–21]. Instead of using a formal devel-opment methodology,
scientists develop their software as follows:</p>

1. The developer forms a basic idea of what is needed and beginscoding.
2. The developer informally evaluates the software through ques-tions like “does this software do what I want?” and
“Can it beusefully extended”?
3. The developer either modifies or extends the code as appropri-ate until the answer to the first question above is
“yes”, and theanswer to the second is “no”.
4.The developer “tests” the software by asking “is the outputbroadly what I expect?”

#### Testing.

T1: The effectiveness of the testing practices currently used by scientific software developers is limited

T2: Scientific software developers would benefit from using a wide range of testing practices from software engineering

T3: The testing practices that scientific software developers do utilize are often executed poorly.

T4: Testing is much more complicated for scientific development than traditional software development since the correct results of a piece of software are frequently not known

####  Verification and Validation

Our survey of the literature identified eleven studies that contained claims about the use of Verification and Validation (V&V) by
scientific software developers. It is worth nothing that software engineers and scientific software developers may have slightly differentunderstandings of V&V. Based on the definitions provided by Babuska and Oden, we provide a mapping between the two domains.
First, software engineers typically understand Validation as the process of ensuring that the project specification (and overall end
product) matches the project goals or user requirements. In scientific software, this same concept is described as ensuring that the
mathematical model (the equivalent of the project specification) matches the real world (the equivalent of the project goals or user
requirements). 
Second, software engineers typically understand Verification as the process of ensuring that the implementation of the software
matches the project specification. In scientific software, this same concept is described as ensuring that the computational model (the
equivalent of the software implementation) matches the mathematical model (the equivalent of the project specification).
We group the detailed list of claims into four over-arching claims in the following discussion.
Table 9, summarizes the four claims that are described in detail below.

--------------------
VV1: The lack of suitable test oracles or comparable software makes validating scientific software difficult

VV2: There are many ways that defects can enter software

VV3: Scientists frequently suspect that any problems in the results of their software result from scientific theory

VV4: Experimental validation is frequently impractical because scientists lack the information they would prefer to use to validate the
software 

VV4: Experimental validation is frequently impractical because scientists lack the information they would prefer to use to vali-
date the software.We found this claim in four studies. There are two primary reasons given for this claim. First, many sci-
entists believe that useful validation would have to consist of comparing the results from their software to the results gained from a
physical experiment or observation. As was mentioned in the introduction, the cost or danger of performing these physical experiments is often the reason why scientists build software models in the first place, so the physical experiments will not be done before promising software models have been created. Second, experimental validation is frequently impractical since it is usually difficult or impossible to know what the correct result for a piece of software will be until the software is run. In some cases, scientific software 
developers treat validation studies as research projects or theses in and of themselves due to the challenge in performing them. In these cases, scientists do not find that it is feasible to fully validate every piece of their software.
