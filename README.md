# relatorio_resumido_SE
Destinado para acrescentar pontos interessantes para o mestrado em SE

<p> modelo de Documentação de software</p>

http://www.riopomba.ifsudestemg.edu.br/dcc/dcc/materiais/938862718_modelo%20de%20documeto%20de%20software.pdf
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

 > VV4: Experimental validation is frequently impractical because scientists lack the information they would prefer to use to vali-
date the software.We found this claim in four studies. There are two primary reasons given for this claim. First, many sci-
entists believe that useful validation would have to consist of comparing the results from their software to the results gained from a
physical experiment or observation. As was mentioned in the introduction, the cost or danger of performing these physical experiments is often the reason why scientists build software models in the first place, so the physical experiments will not be done before promising software models have been created. Second, experimental validation is frequently impractical since it is usually difficult or impossible to know what the correct result for a piece of software will be until the software is run. In some cases, scientific software 
developers treat validation studies as research projects or theses in and of themselves due to the challenge in performing them. In these cases, scientists do not find that it is feasible to fully validate every piece of their software.

#### Documentation

<p> Documentation produced by developers</p>
 
+ +/- 84% Code Comments
+ 70% User Manuals/Guides
+ 50% Installation Guides
+ +/- 45% Theory/Algorithm Descriptions
+ +/- 45% Test Results
+ 40% Design Documentation
+ 30% Requirements Documentation

D1: Documentation is a necessary enabler of software quality

D2: Documentation is becoming more frequently used

D3: Documentation requires a significant investment of work


> D1: Documentation is a necessary enabler of software quality. Formal documents are important when a project is given to a team
that is not the original development team. In fact, examinations of the ASCI program at LANL and Lawrence Livermore National Laboratory (LLNL) suggest that documentation is one of the practices that is essential for scientific software developers to adopt in order to guarantee quality. One benefit is that documentation enables communication between team members as well as providing references for papers, grant authoring, and grant reporting. Documentation is especially vital if scientific software developers wish to use their earlier software as a basis for developing more advanced software.

> D2: Documentation is becoming more frequently used. In a more recent study, Nguyen-Hoan et al.conclude, based on the result of a survey with 60 respondents, that documentation is more widely produced than is indicated in these early studies. The responses to their summary are given in... Nguyen-Hoan et al. also gave the three most common arguments in favor of producing comments as well as the four most common reasons for not producing comments. The comments in favor were: (1) “For users of the software”, (2) “For future maintenance purposes”, and (3) “Documentation is integral to software.” The arguments against documentationwere: (1) “Limited due to time and effort required”, (2) “Effort not worth it due to small user base”, (3) “requirements constantly changing or not specified up front,” and (4) “Software should be or is ‘intuitive’, ‘easy to understand’, or ‘doesn’t need a full description’

> D3: Documentation requires a significant investment of work. Not all of the claims about documentation were positive. The effort
required to create documentation leads some developers to conclude hat scientific software developers should be careful about how much
documentation they create. Furthermore, if the documentation is done to satisfy an external requirement it may not benefit
the project team. However, one study did find an alternative to performing a separate documentation task and utilized an automatic documentation generator that creates documentation from comments in the project’s source files.

#### Issue tracking

IT1: Issue tracking greatly eases communication between members of a development team.

IT2: Issue tracking helps insure that no two groups in a development team are working on the same problem

> IT1: Issue tracking greatly eases communication between members of a development team. Issue tracking is a useful practice
for communicating information about discovered bugs and needed functionality between developers. Issue tracking software allows this
information to be stored and communicated instantly between all members of a development team. When additional remote groups
are added to existing development teams, an issue tracking system is required to formally record bugs and new requirements as well as
to create a trail of the completed activity. Issue-tracking software also made a list of the ten most important software engineering
practices for scientific software developers to use. There are four primary reasons to use issue tracking software rather than informally tracking issues:

> + Issues can be made visible to the entire team

> + The ability to prioritize issues is frequently provided Many systems provide the ability to track dependencies between 
issues; and

> + The history of issues is searchable for future reference

> IT2: Issue tracking helps insure that no two groups in a development team are working on the same problem.
The dependency tracking feature of issue tracking software also allows a large deliverable to be broken into a set of smaller features that it is dependent upon. This set can then be distributed among various groups so that no two groups are working on the same feature.


#### Version control

VC1: Version control software is necessary for research groups with more than one developer

VC2: Distributed version control is particularly useful for scientific software development


 > VC1: Version control software is necessary for research groups with more than one developer.
Version control tools are needed to keep up with changes to software that can accumulate extremely rapidly. Version control tools allow a developer to track each new version of a piece of code that is created and identify changes between versions.
Versions of software that are used to publish results, support major decisions, or undergo extreme testing are the most important to track. In addition, the developer needs to maintain a complete copy of any software used to produce important results. An example of
why the need to keep a copy of the software is important is a case where a researcher tried to reproduce results that she had produced
the previous year. Because the researcher did not have access to the old versions of the data she needed, she had to spend a considerable amount of time reproducing the input data. In one case, even though she had the data, the results were significantly different from the previous run. In this case, the executable for the first test had been built using different compiler options. 
In addition to utilizing version control systems, it is useful to have a formal process to approve code that is to be checked into the repository. This process would ensure that a piece of code passes all relevant test cases instead of relying on individual developers to perform these tests.

VC2: Distributed Version Control is particularly useful for scientific software development. There are two major types of version
control systems: centralized and distributed. In a centralized system, a single server stores the master copy of the entire project; meaning that if the server goes down or the network becomes unavailable, no one can submit work on the project. Also, if the server’s data is lost, the entire project is lost as well. An alternative is to use a distributed version control system instead. In this implementation, each user has a full copy of the entire project on their machine which is updated to match other copies as connections to the other nodes in the network are available. The primary problem with distributed version control systems is that they are complicated to manage, requiring a strategy for sharing modifications and synchronizing local copies.One instance of distributed version control is “The Abinit forge”, a custom version control system built on Bazaar–a distributed version control system and an ssh-server. Each Abinit developer has a Bazaar repository that stores their branches of their software, providing fast data access and somewhat optimized usage of disk space. A daily script makes all contributions to a project available through a password-protected website which allows the developer to share his work with others and organize collaborative developments involving remote workplaces. Other tools in common use are: Revision Control System and Concurrent Version System, the latter of which can be utilized from within the Eclipse IDE to ease the overhead required by adopting the tool.

### Conclusões tiradas a partir da leitura do paper

---

Com base no que foi abordado durante o paper **Claims about the use of software engineering practices in science: a systematic literature review**, podemos salientar alguns aspectos interessantes que possa ser útil na elaboração de um mestrado futuro. No quesito de teste de softwares cientificos, alguns dos entrevistados mencionou a falta de apoio da gestão, no tocante de garantir a qualidade dos testes e mostrar a eficiencia de sua aplicação, levando em conta se os resultados apresentados são confiáveis para comparação com um modelo padrão. Uma boa pratica apresentada pelo paper foi a de criar um metodologia de testes para evitar bugs no decorrer da elaboração do código, é desenvolver uma construção regular e automatizada para testar seu código regularmente, evitando assim a espera do produto final para assim realizar os testes. Dois métodos foram citados no paper: testes de regressão e testes de integração, onde foi citado que os cientistas utilizam muito o teste de integração. apresentando o seguinte exemplo: "os cientistas o tratam como um novo experimento e o testam, usando os resultados anteriores como um controle."

Partindo para o tópico de Validação e Verificação, constatamos uma diferença no conceito de V&V entre Engenheiro de Software (EG) e Desevolvedores de Software Cientificos(DSC). Enquanto que o EG lida com a validação a rigor de assegurar a especificação esteja de acordo com as metas; o DSC precisa assegurar que o modelo matemático esteja dentro das condições do mundo real. Na verificação, o EG precisa garantir a implementação do produto, enquanto que o DSC é garantir que o que foi implementado corresponde ao modelo matemático. Pegando o ponto de vista de validação de um desenvolvedor de software cientifico, constatamos que isso não é muito praticado pelos cientisitas devido a falta de informação, por não possuir todos os resultados esperados durante todo o software. Com isso os cientistas não constumam validar todo o software, somente os pontos que possí experimentos viáveis para a comparação.

Uma visão geral no quesito de documentação elaborada pelos desenvolvedores, podemos notar que a maioria adota a pratica de adicionar comentários no decorrer da criação do software; seguido pela pratica de manuais e guias para os usuários e em seguida pela guia de instalação. A descrição de teoria e algoritmo e resultado dos testes, alcançou a mesma quantidade (ponto que acredito ser uma boa pratica apenas na criação de paper, dissertação e teses). A documentação de design e requisitos, são praticas pouco realizada pelos desenvolvedores.
