---
layout: default
title: "Open topics"
has_toc: true
nav_order: 2
---

# Open topics
{: .no_toc }

The following topics are currently open for Bachelor's and Master's thesis.

## Overview
{: .no_toc .text-delta }

- TOC
{:toc}

## \#awesome: A Review and Clustering Analysis of Awesome Lists on GitHub
{: .d-inline-block }
#literature-review
{: .label .label-yellow }
#data-science
{: .label .label-green }

**Thesis Advisor**: Prof. Dr. Gerit Wagner

**Summary**: This thesis focuses on the increasingly popular “awesome lists” on GitHub, which represent an informal but useful method of knowledge collection and synthesis. The goal of the thesis is to use the colrev package to automatically retrieve relevant repositories from GitHub, and subsequently conduct a clustering analysis to distinguish between different types of awesome lists. Categories of awesome lists might include those focusing on datasets, academic publications, or non-academic use cases. The thesis should provide an overview of the landscape of awesome lists, identify prominent examples, and derive best practice recommendations for designing these resources. Furthermore, the thesis will suggest potential ways academia could leverage awesome lists for literature reviews and contribute to their development.

**Methods**: The thesis will employ the colrev package for retrieving and processing GitHub repositories and apply clustering techniques to categorize the awesome lists. Both qualitative and quantitative analyses will be used to identify interesting patterns across the lists. 

**Expected outcomes**: The thesis will result in a comprehensive classification of awesome lists on GitHub, with detailed examples of exemplary lists. It will also provide recommendations on how best to design such lists for different audiences and use cases, including guidance for future academic involvement in these lists. Furthermore, the research will suggest how awesome lists can be applied in systematic literature reviews and knowledge synthesis in academic settings.

**Requirements**: Students should have basic experience with GitHub and Python, particularly in data retrieval and analysis. Familiarity with clustering techniques or the colrev package is an advantage.

**References**

<div class="references">
  <p>Sindresorhus (2023). Awesome Lists. Available at <a href="https://github.com/sindresorhus/awesome" target="_blank">https://github.com/sindresorhus/awesome</a>.</p>
  <p>Gusenbauer, M., & Haddaway, N. R. (2021). What every researcher should know about searching–clarified concepts, search advice, and an agenda to improve finding in academia. <em>Research Synthesis Methods</em>, 12(2), 136-147.</p>
<p>Nakagawa, S., Dunn, A. G., Lagisz, M., Bannach-Brown, A., Grames, E. M., Sánchez-Tójar, A., ... & Haddaway, N. R. (2020). A new ecosystem for evidence synthesis. <em>Nature Ecology & Evolution</em>, 4(4), 498-501. <a href="https://doi.org/10.1038/s41559-020-1153-2" target="_blank">https://doi.org/10.1038/s41559-020-1153-2</a>.</p>
</div>

<!--

{: .info}
**There are not open topics at the moment. New topics will be announced shortly.**

{: .call_for_theses }
Topis that are part of the **#SEARCH-QUERY** call-for-theses are marked with a label. They should be completed between August 2024 and December 2024. Students participating in this call are invited to review each of the others work after two months, and to contribute their work to the [search-query](https://github.com/CoLRev-Environment/search-query){: target="_blank"} project. The project will be submitted to a journal, such as the [Journal of Open Source Software](https://joss.theoj.org/about){: target="_blank"}, giving students the opportunity to become a co-author on a peer-reviewed paper.

<div class="page-break"></div>

## Design of an emulator for API-based academic literature searches
{: .d-inline-block }
#programming
{: .label .label-yellow }
#search-query
{: .label .label-green }

**Thesis Advisor**: Prof. Dr. Gerit Wagner

**Summary**: This thesis aims to advance the use of Boolean queries (queries involving operators like AND, OR, NOT) in API searches in two areas. First, for a suitable API (e.g., PubMed), a parser will be implemented for URLs representing Boolean queries. This will extend existing functionality of the [search-query](https://github.com/CoLRev-Environment/search-query){: target="_blank"} package and allow users to efficiently run Boolean queries when the API supports it. Second, for APIs that do not support Boolean queries (such as Crossref or DBLP), a novel technique, called *Boolean Emulation for Academic Literature Searches* (BEALS), will be implemented and tested. For this technique, which involves the retrieval of super-sets followed by local execution of Boolean queries, a concept and working prototype are available.

**Methods**: The thesis will adopt a design science approach and proceed in two phases: 1) Parsing query URLs for APIs that already support nested Boolean queries. 2) Developing and implementing the BEALS technique for APIs lacking Boolean operator support, followed by user tests.

**Expected outcomes**: The thesis will provide an extension of the search-query package, demonstrating improved search capabilities for both types of APIs. It will include the design of the BEALS technique, showcasing its ability to emulate Boolean functionalities for simple APIs. These contributions will enhance efficiency of literature searches, ultimately allowing researchers to rely on automated execution instead of manual retrieval from database interfaces.

**Requirements**: Candidates should have completed the [open-source project](https://digital-work-lab.github.io/open-source-project/){: target="_blank"} or have prior experience with Git and Python.

**References**

<div class="references">
  <p>Gusenbauer, M., &amp; Haddaway, N. R. (2021). What every researcher should know about searching–clarified concepts, search advice, and an agenda to improve finding in academia. <em>Research Synthesis Methods</em>, 12(2), 136-147.</p>
  <p>Peffers, K., Tuunanen, T., Rothenberger, M. A., &amp; Chatterjee, S. (2007). A design science research methodology for information systems research. <em>Journal of Management Information Systems</em>, 24(3), 45-77. <a href="https://www.tandfonline.com/doi/abs/10.2753/MIS0742-1222240302">link</a></p>
  <p>Wagner, G., & Ernst, K. M. (2024). Search-query: A Python package for queries in academic literature searches. (Version 0.10.0) [Computer software]. https://github.com/ColRev-Environment/search-query<a href="https://github.com/ColRev-Environment/search-query">https://github.com/ColRev-Environment/search-query</a></p>
</div>

<div class="page-break"></div>

## Advances in literature search queries: Evaluation, analysis, and improvement
{: .d-inline-block }
#programming
{: .label .label-yellow }
#search-query
{: .label .label-green }

**Thesis Advisor**: Prof. Dr. Gerit Wagner

**Summary**: This thesis focuses on literature search queries, and aims to evaluate, analyse, and improve them.
As a first step, a comprehensive dataset from [searchRxiv](https://www.cabidigitallibrary.org/journal/searchrxiv){: target="_blank"} will be used to parse and evaluate queries for selected databases (such as Web of Science, Pubmed, or IEEE).
This step relies on existing query parsers, may involve refinements of the parser, and ultimately classify each query as valid or erroneous.
As the second step, a linter will be extended to identify different types of problems and offer instructive messages to users.
This work will proceed from syntactical errors (e.g., unbalanced parentheses) to simplification techniques (e.g., use of of wildcards).
We will assist students with the development of a code skeleton (if needed).

**Methods**: The thesis will adopt a design science approach and proceed in two phases: 1) Creating a test dataset of queries based on searchRxiv. 2) Implementing linters, testing them on the dataset, and reporting the results.

**Expected outcomes**: The thesis will verify the functionality of parsers within the search-query package, and develop linters for analyzing and simplifying queries. Based on an analysis of data from searchRxiv, it will further show whether published queries have errors or whether they could be simplified.

**Requirements**: Candidates should have completed the [open-source project](https://digital-work-lab.github.io/open-source-project/){: target="_blank"} or have prior experience with Git and Python.

**References**

<div class="references">
  <p>Gusenbauer, M., &amp; Haddaway, N. R. (2021). What every researcher should know about searching–clarified concepts, search advice, and an agenda to improve finding in academia. <em>Research Synthesis Methods</em>, 12(2), 136-147.</p>
  <p>Sturm, B., &amp; Sunyaev, A. (2019). Design principles for systematic search systems: a holistic synthesis of a rigorous multi-cycle design science research journey. <em>Business &amp; Information Systems Engineering</em>, 61, 91-111.</p>
  <p>Wagner, G., & Ernst, K. M. (2024). Search-query: A Python package for queries in academic literature searches. (Version 0.10.0) [Computer software]. https://github.com/ColRev-Environment/search-query<a href="https://github.com/ColRev-Environment/search-query">https://github.com/ColRev-Environment/search-query</a></p>
</div>

<div class="page-break"></div>

## Advances in search query tools: A comprehensive evaluation
{: .d-inline-block }
#programming
{: .label .label-yellow }
#search-query
{: .label .label-green }

**Thesis Advisor**: Prof. Dr. Gerit Wagner

**Summary**: This thesis focuses on search query tools, and aims to evaluate how they handle complex queries, and whether there are any limitations.
Similar to the previous topic, in the first step, a comprehensive dataset from [searchRxiv](https://www.cabidigitallibrary.org/journal/searchrxiv){: target="_blank"} will be used to parse and evaluate queries for selected databases (such as Web of Science, Pubmed, or IEEE).
This step relies on existing query parsers, may involve refinements of the parser, and ultimately classify each query as valid or erroneous.
In the second step, existing search query tools, such as *Polyglot Search* or *Litsonar*, will be evaluated based on this dataset of queries.
The goal is to scrutinize their ability to parse free-text queries, and the formats available for translation. For each tool, it will be analysed whether complex queries with a valid syntax are parsed correctly and without errors, and whether erroneous queries are rejected.
Finally, the research will also involve reporting any identified errors to the developers.

**Methods**: The thesis will adopt a design science approach and proceed in three phases: 1) Creating a test dataset of queries based on searchRxiv. 2) Testing valid and erroneous queries in different tools. 3) Documenting errors, sharing them with the developers, and reporting whether the developers responded or fixed the errors (considering the time frame available for the thesis).

**Expected outcomes**: The thesis will provide a detailed evaluation of the capabilities and limitations of existing search query tools. It will highlight the strengths and weaknesses of each tool, provide insights into the most common issues encountered, and assess the responsiveness of developers in addressing reported errors. This work will contribute to the improvement of search query tools and offer practical recommendations for developers and users.

**Requirements**: Candidates should have completed the [open-source project](https://digital-work-lab.github.io/open-source-project/){: target="_blank"} or have prior experience with Git and Python.

**References**

<div class="references">
  <p>Aguinis, H., Ramani, R. S., & Alabduljader, N. (2023). Best-practice recommendations for producers, evaluators, and users of methodological literature reviews. <em>Organizational Research Methods</em>, 26(1), 46-76. doi:10.1177/109442812094328</p>
  <p>Gusenbauer, M., & Haddaway, N. R. (2021). What every researcher should know about searching–clarified concepts, search advice, and an agenda to improve finding in academia. <em>Research Synthesis Methods</em>, 12(2), 136-147.</p>
  <p>Sturm, B., & Sunyaev, A. (2019). Design principles for systematic search systems: a holistic synthesis of a rigorous multi-cycle design science research journey. <em>Business &amp; Information Systems Engineering</em>, 61, 91-111.</p>
  <p>Wagner, G., & Ernst, K. M. (2024). Search-query: A Python package for queries in academic literature searches. (Version 0.10.0) [Computer software]. https://github.com/ColRev-Environment/search-query<a href="https://github.com/ColRev-Environment/search-query">https://github.com/ColRev-Environment/search-query</a></p>
  <p>Polyglot Search documentation. Available at <a href="https://polyglot.sr-accelerator.com/" target="_blank">https://polyglot.sr-accelerator.com/</a>.</p>
  <p>LitSonar project details. Available at <a href="https://litsonar.com" target="_blank">https://litsonar.com</a>.</p>
  <p>SearchRefineR project details. Available at <a href="https://ielab.io/searchrefiner/tools/" target="_blank">https://ielab.io/searchrefiner/tools/</a>.</p>
</div>

## Generative artificial intelligence and archetype prompts in software development: A scoping review

**Thesis Advisor**: Prof. Dr. Gerit Wagner

**Summary**: The advent of generative artificial intelligence (AI) has revolutionized the landscape of software development, offering new ways to automate and optimize the coding process. This thesis seeks to explore the burgeoning domain of generative AI, particularly focusing on how archetype prompts can effectively guide AI to produce more efficient, reliable, and sophisticated software solutions. The objective is to conduct a comprehensive scoping review to map the extent, range, and nature of research activity in this area, identify gaps in the current literature, and consolidate knowledge about the types and effectiveness of archetype prompts in guiding generative AI in software development. Key questions include: What are the prevailing types of archetype prompts used in generative AI for software development? What are the outcomes associated with different prompt types? And how do these prompts influence the software development process and its outcomes?

**Methods**: Scoping review methodology (covering academic and grey literature)

**Expected outcomes**: The thesis will provide a detailed map of the existing academic discourse on the use of generative AI and archetype prompts in software development. It will identify key themes, methodologies, and findings across the literature, outline the benefits and limitations of various approaches, and suggest areas for future research. The review will also critically assess the quality of the current research and provide recommendations for incorporating archetype prompts into generative AI systems to optimize software development processes.

**References**

Arksey, H., & O'Malley, L. (2005). Scoping studies: towards a methodological framework. *International Journal of Social Research Methodology*, 8(1), 19-32.

Hou, X., Zhao, Y., Liu, Y., Yang, Z., Wang, K., Li, L., ... & Wang, H. (2023). Large language models for software engineering: A systematic literature review. *arXiv preprint* arXiv:2308.10620.

OpenAI (2023) OpenAI Cookbook. Available at [https://cookbook.openai.com/](https://cookbook.openai.com/){: target="_blank"}.

OpenAI (2023) Prompt engineering guide. Available at [https://platform.openai.com/docs/guides/prompt-engineering](https://platform.openai.com/docs/guides/prompt-engineering){: target="_blank"}

Saravia, Elvis (2022) Promp Engineering Guide. Available at [https://www.promptingguide.ai/de](https://www.promptingguide.ai/de){: target="_blank"}.

White, J., Hays, S., Fu, Q., Spencer-Smith, J., & Schmidt, D. C. (2023). ChatGPT prompt patterns for improving code quality, refactoring, requirements elicitation, and software design. *arXiv preprint* arXiv:2303.07839.


## Careers in IT: A synthesis of prior research on career paths 

**Thesis Advisor**: Prof. Dr. Gerit Wagner

**Summary**: This thesis aims to provide a comprehensive synthesis of existing research on career paths in Information Technology (IT), accompanied by a critical review of the methodologies employed in these studies. It will explore the evolution and nature of IT careers, the impact of technological advancements, and the role of education and organizational structures in shaping these career paths. The thesis will not only consolidate knowledge about the career trajectories and factors influencing them but also critically examine the research methodologies used in prior studies to assess their rigor, limitations, and implications. This critical review will help identify potential biases, gaps, and areas for improvement in IT career research, thereby providing a foundation for future inquiries.

**Methods**: Critical literature review methods

**References**

Aguinis, H., Ramani, R. S., & Alabduljader, N. (2023). Best-practice recommendations for producers, evaluators, and users of methodological literature reviews. *Organizational Research Methods*, 26(1), 46-76.

Idowu, A., & Elbanna, A. (2020). Digital platforms of work and the crafting of career path: the crowdworkers’ perspective. *Information Systems Frontiers*, 24, 441-457.

Joia, L. A., & Mangia, U. (2017). Career transition antecedents in the information technology area. *Information Systems Journal*, 27(1), 31-57.

Joseph, D., Boh, W. F., Ang, S., & Slaughter, S. A. (2012). The career paths less (or more) traveled: A sequence analysis of IT career histories, mobility patterns, and career success. *MIS Quarterly*, 36(2), 427-452.


## Ethical challenges and regulatory responses in gig work: An analysis of emergent policy agendas

**Thesis Advisor**: Prof. Dr. Gerit Wagner

**Summary**: The gig economy, characterized by short-term contracts and freelance work as opposed to permanent jobs, has transformed the labor market. This thesis aims to explore the ethical challenges inherent in gig work and analyze the regulatory responses aimed at addressing these issues. Students will investigate the precarious nature of gig work, including issues related to workers' rights, employment benefits, and income stability. The research may also encompass the broader societal and economic implications of gig work, such as its impact on traditional employment and social security systems. Furthermore, this thesis will critically analyze emergent policy agendas and regulatory frameworks from various global contexts, assessing their effectiveness in safeguarding gig workers' rights and promoting fair labor practices.

**Methods**: Scoping review and policy analysis

**Expected outcomes**: The thesis will provide a comprehensive comparative analysis of regulatory measures and policy agendas addressing the ethical challenges of gig work across different regions and countries. It will identify and articulate the common themes, strategies, and objectives present in these regulations, as well as highlight the significant differences in approach and focus that arise from varying economic, cultural, and political contexts. This comparison will allow for a deeper understanding of the effectiveness and limitations of different regulatory strategies, offering insights into best practices and lessons learned from various jurisdictions. Ultimately, the thesis will contribute to the development of more nuanced and effective policy frameworks for the gig economy, taking into account the diverse needs and circumstances of gig workers globally.

**References**

Arksey, H., & O'Malley, L. (2005). Scoping studies: towards a methodological framework. *International Journal of Social Research Methodology*, 8(1), 19-32.

Deng, X., Joshi, K. D., & Galliers, R. D. (2016). The duality of empowerment and marginalization in microtask crowdsourcing. *MIS Quarterly*, 40(2), 279-302.

Graham, M., Woodcock, J., Heeks, R., Mungai, P., Van Belle, J. P., du Toit, D., & Silberman, S. M. (2020). The Fairwork Foundation: Strategies for improving platform work in a global context. *Geoforum*, 112, 100-103.

Myhill, K., Richards, J., & Sang, K. (2021). Job quality, fair work and gig work: the lived experience of gig workers. *The International Journal of Human Resource Management*, 32(19), 4110-4135.


## Translating research findings for online labor markets: A realist review
{: .d-inline-block }
#literature-review
{: .label .label-green }

**Thesis Advisor**: Prof. Dr. Gerit Wagner

**Summary**: Online labor markets, such as Upwork, Fiverr, and 99designs, are reshaping the nature of work, employment, and income generation across the globe. This thesis aims to perform a realist review of the literature focusing on the translation of research findings into practical and actionable strategies for various stakeholders in online labor markets, including workers, clients, platform providers, and policymakers. It will examine the contextual factors and mechanisms that influence the successful application of academic insights, exploring how these stakeholders can leverage research to optimize outcomes, enhance fair practices, and ensure sustainable growth of the labor market. The review will dissect the interplay between these stakeholders, understanding their roles, motivations, and the outcomes of their interactions in the digital labor ecosystem.

**Methods**: Realist Review

**Expected outcomes**: The thesis will provide a thorough analysis identifying strategies that effectively translate research into practice for all stakeholders involved in online labor markets. It will clarify the conditions and mechanisms that lead to successful outcomes for workers, such as improved job security and satisfaction; for clients, such as enhanced service quality and efficiency; for platform providers, including increased user engagement and market share; and for policymakers, involving the creation of more effective and equitable regulations. This comprehensive understanding will offer a framework for stakeholders to make informed decisions and implement evidence-based strategies. Additionally, it will pinpoint gaps and suggest future research directions to continually enhance the functioning and governance of online labor markets.

**References**

<div class="references">
  <p>Barach, M. A., Golden, J. M., & Horton, J. J. (2020). Steering in online markets: the role of platform incentives and credibility. *Management Science*, 66(9), 4047-4070.</p>
  <p>Horton, J. J. (2019). Buyer uncertainty about seller capacity: Causes, consequences, and a partial solution. *Management Science*, 65(8), 3518-3540.</p>
  <p>Huang, N., Burtch, G., Hong, Y., & Pavlou, P. A. (2020). Unemployment and worker participation in the gig economy: Evidence from an online labor market. *Information Systems Research*, 31(2), 431-448.</p>
  <p>Liang, C., Hong, Y., Gu, B., & Peng, J. (2018). Gender wage gap in online gig economy and gender differences in job preferences. In *Proceedings of the 39th International Conference on Information Systems*.</p>
  <p>Pawson, R., Greenhalgh, T., Harvey, G., & Walshe, K. (2005). Realist review-a new method of systematic review designed for complex policy interventions. *Journal of Health Services Research & Policy*, 10(1), 21-34.</p>
</div>

## Exploring the role of micro-credentials for online labor markets: An organizing review
{: .d-inline-block }
#literature-review
{: .label .label-green }

**Thesis Advisor**: Prof. Dr. Gerit Wagner

**Summary**: In the evolving landscape of online labor markets, micro-credentials can be a crucial tool for workers to demonstrate their skills, knowledge, and competencies to potential clients. This thesis aims to conduct an organizing review of the existing literature on micro-credentials, focusing on their role in online labor markets. It will explore how these certifications are perceived and used by various stakeholders, including workers, clients, and platform providers. The review will investigate the impact of micro-credentials on employability, job performance, and market dynamics, examining how they contribute to the professional development of individuals and the overall functioning of digital work platforms.

**Methods**: Organizing Review

**Expected outcomes**: The thesis will provide a structured synthesis of the literature on micro-credentials, identifying key themes, trends, and gaps in the research. It will elucidate the role of micro-credentials in enhancing the transparency, trust, and efficiency of online labor markets, as well as their potential limitations and challenges. The work will offer insights into the best practices for designing, implementing, and recognizing micro-credentials, providing recommendations for workers, platform providers, and policymakers. By bringing clarity and organization to the diverse body of research on this topic, the thesis will contribute to a better understanding of how micro-credentials can be leveraged to improve outcomes for all stakeholders in online labor markets.

**References**

Ahmat, N. H. C., Bashir, M. A. A., Razali, A. R., & Kasolang, S. (2021). Micro-credentials in higher education institutions: Challenges and opportunities. *Asian Journal of University Education*, 17(3), 281-290.

Leidner, D. E. (2018). Review and theory symbiosis: An introspective retrospective. *Journal of the Association for Information Systems*, 19(6), 1.

McGreal, R., & Olcott Jr, D. (2022). A strategic reset: micro-credentials for higher education leaders. *Smart Learning Environments*, 9(1), 9.

## Working in diametrically opposed contexts: An exploratory study of commercial open-source developers
{: .d-inline-block }
#literature-review
{: .label .label-green }

**Thesis Advisor**: Prof. Dr. Gerit Wagner

**Summary**: The rise of commercial open-source projects presents a unique juxtaposition of community-driven and commercially-driven development paradigms. This thesis seeks to explore the experiences of developers in these dual contexts, focusing particularly on the role of worker identity in navigating the tensions between open-source collaboration and commercial objectives. It aims to understand how developers reconcile their professional, personal, and community identities while working under the contrasting demands of open-source ethos and commercial profitability. The study will delve into how identity influences motivations, engagement, conflict management, and overall strategies in the commercial open-source environment.

**Methods**: Scoping review, covering academic and grey literature

**Expected outcomes**: The thesis will offer a detailed exploration of how commercial open-source developers perceive and manage their multifaceted identities in the face of divergent work paradigms. It will uncover the implications of these identity dynamics on collaboration, innovation, and conflict within open-source projects that have commercial aims. The work will highlight how identity shapes developers' approaches to their work and interactions with the community and commercial entities. By elucidating these identity aspects, the thesis will provide deeper insights into the challenges and strategies of developers, contributing to more effective management and support structures in hybrid open-source models.

**References**

Alexy, O., Henkel, J., & Wallin, M. W. (2013). From closed to open: Job role changes, individual predispositions, and the adoption of commercial open source software development. *Research Policy*, 42(8), 1325-1340.

Andersen-Gott, M., Ghinea, G., & Bygstad, B. (2012). Why do commercial companies contribute to open source software?. *International Journal of Information Management*, 32(2), 106-117.

Henkel, J. (2009). Champions of revealing—the role of open source developers in commercial firms. *Industrial and Corporate Change*, 18(3), 435-471.

Shahrivar, S., Elahi, S., Hassanzadeh, A., & Montazer, G. (2018). A business model for commercial open source software: A systematic literature review. *Information and Software Technology*, 103, 202-214.

## Future of Work: A review of reviews

**Thesis advisor**: Prof. Dr. Gerit Wagner

**Summary**: In recent years, we have seen a tremendous growth of research dedicated to the future of work, covering topics like the transition to remote work, emerging forms of online labour, as well as (techno) stress and well-being. An effective transfer of scientific findings into practice is challenged by the unprecedented volume of research studies published each year. In this context, integrated overviews of existing research are essential to properly inform managerial stakeholders on the key areas and topics investigated by academia. Such work can also offer useful guidance and shape the agendas of researchers. The goal of this thesis is to provide an overview of prior research related to the future of work, focusing on prior review papers exclusively. For example, the reviews of Marsh et al. (2022), Mitchell et al. (2022), and Gol2019 cover relevant facets. More generally, the objective would be to use available guidelines (Thomson et al. 2010), search for review papers on digital work, complete a structured selection process (screen), and synthesize the key findings adopting a concept-centric perspective (see Webster and Watson 2000). Relevant implications for practice and research conclude the thesis.

**Method**: Literature review (qualitative)

**References**

Gol, E. S., Stein, M. K., & Avital, M. (2019). Crowdwork platform governance toward organizational value creation. The Journal of Strategic Information Systems, 28(2), 175-195.

Marsh, E., Vallejos, E. P., & Spence, A. (2022). The digital workplace and its dark side: An integrative review. Computers in Human Behavior, 128, 107118.

Mitchell, R., Shen, Y., & Snell, L. (2022). The future of work: a systematic literature review. Accounting & Finance, 62(2), 2667-2686.

Thomson, D., Russell, K., Becker, L., Klassen, T., & Hartling, L. (2010). The evolution of a new publication type: steps and challenges of producing overviews of reviews. Research synthesis methods, 1(3‐4), 198-211.

Webster, J., & Watson, R. T. (2002). Analyzing the past to prepare for the future: Writing a literature review. MIS quarterly, xiii-xxiii.

## Online labour markets: Key constructs, items, and nomological network

**Thesis advisor**: Prof. Dr. Gerit Wagner

**Summary**: Online labour markets enable clients to hire individual workers, often for short-time contracts and tasks ranging from programming to translation services, and online marketing campaigns. Global demand for professional services on online labour markets is growing, but the experience of clients is not always satisfactory. In fact, clients fail to find suitable candidates for less than 75% of jobs in projects exceeding 1,000$ (Snir and Hitt, 2003). Prior research has invested considerable efforts to identify constructs explaining selection decisions and auction success (Wagner and Prester, 2021). Examples for explanatory constructs are worker experience, ratings, and cultural similarity. Yet, we lack an overview of how these constructs are measured (their items) and how they are related to each other in a nomological network. Developing a more systematic overview of the key constructs can draw inspiration from similar studies (e.g., Clark et al., 2007, Zhang and Venkatesh, 2017) and methodological works (e.g., Larsen et al. 2016; Larsen et al. 2020). Such a contribution is important to ensure nomological validity in future studies, to facilitate better compatibility of individual studies, and to achieve higher predictive accuracy, potentially helping clients to utilize online labour markets more effectively.

**Method**: literature synthesis (qualitative and/or quantitative)

**References**

Clark Jr, T. D., Jones, M. C., & Armstrong, C. P. (2007). The dynamic structure of management support systems: theory development, research focus, and direction. MIS Quarterly, 31(3), 579-615.

Larsen, K. R., & Bong, C. H. (2016). A tool for addressing construct identity in literature reviews and meta-analyses. Mis Quarterly, 40(3), 529-552.

Larsen, K., Gefen, D., Petter, S., & Eargle, D. (2020). Creating Construct Distance Maps with Machine Learning: Stargazing Trust. In: Proceedings of the Americas Conference on Information Systems.

Prester, J., & Wagner, G. (2021). Contracting Decisions on Digital Markets for Knowledge Work Services: A Qualitative Systematic Review. In: Proceedings of the International Conference on Information Systems.

Snir, E. M., & Hitt, L. M. (2003). Costly bidding in online markets for IT services. Management Science, 49(11), 1504-1520.

Zhang, X., & Venkatesh, V. (2017). A nomological network of knowledge management system use: Antecedents and consequences. MIS quarterly, 41(4), 1275-1306.


Literature reviews: Conceptual models and tools for inductive and theoretical work

Literature reviews in the Information Systems as well as the Management and Organizational Disciplines often adopt inductive approaches for synthesis and theory development. This means that authors approach prior reseach with an open mind and let concepts and associations emerge from the analysis (see Wolfswinkel et al., 2013). This differs from deductive approaches in which a specific schema is selected at the beginning and applied to the literature. Inductive work is considered to be particularly valuable because it allows authors to draw new insights from extant work. Yet, it is also considered particularly challenging to complete inductive reviews from a conceptual and practical perspective. Conceptually, a well-known guideline suggests to develop a concept matrix (Webster and Watson, 2001), but less than 10% of theoretical reviews in Information Systems strictly follow this approach. Similarly, there is a lack of guidelines on appropriate tools and how they can support inductive reviews.

The goal of this thesis is to offer conceptual and practical guidance for inductive literature reviews. Conceptually, this could involve an analysis of inductive review papers and current guidelines, including Webster and Watson’s concept matrix, Glaser and Strauß’s Grounded Theory, or Luhmann’s method. Practically, it may be helpful to review available tools, such as MAXDQA, Atlas.TI, Obsidian, or Zettlr, and to simulate inductive work (in line with example review papers). This work should have implications for future inductive and concept-centric reviews, for instance in the form of archetype patterns, methodological propositions, or guidelines for tools.

Method: Literature review and analysis, tool evaluation

References

Bandara, W., Furtmueller, E., Gorbacheva, E., Miskon, S., & Beekhuyzen, J. (2015). Achieving rigor in literature reviews: Insights from qualitative data analysis and tool-support. Communications of the Association for Information systems, 37(1), 8.

Glaser, B. G., & Strauss, A. L. (2008). Grounded theory: strategien qualitativer forschung. Huber.

Webster, J., & Watson, R. T. (2002). Analyzing the past to prepare for the future: Writing a literature review. MIS Quarterly, 26(2), xiii-xxiii.

Wolfswinkel, J. F., Furtmueller, E., & Wilderom, C. P. (2013). Using grounded theory as a method for rigorously reviewing literature. European Journal of Information Systems, 22(1), 45-55.


##  Data science: Design and evaluation of a machine learning classifier for information retrieval

To present users with the most relevant results in information retrieval and collaborative filtering settings, it is imperative to go beyond pure network structure and consider qualitative and (semi-) structured data (Herlocker et al. 2004). For example, a social media-post or newspaper article will be considered more relevant if it matches a users context and the topics s/he is interested in. This notion of relevance may not only be inferred from the original document, but also from others who refer to it (e.g., in the form of mentions and reviews). The objective of this thesis is to leverage data from referring documents to predict which of the original documents are relevant to a user.

The thesis will focus on the context of academic citation networks in which researchers are challenged to evaluate thousands of papers (original documents) to select those relevant to their work (see Prester et al. 2021). An existing data set will be provided (based on Wagner et al. 2021), which contains the network structure, the referring documents, as well as labels of relevance. The referring documents are in TEI formats (generated from PDFs), which allows for an efficient access of referring sections (contents, citations, and context). These structural and semi-structured data elements should be used to develop features as well as to implement and evaluate a machine learning classifier. Ultimately, such classifiers could help to offer more efficient alternatives to what is commonly known as snowballing, citation, or backward searches (Choong et al., 2014, Webster and Watson, 2001).

Methods: Machine learning (feature engineering, model development, evaluation)

Prerequisites: Programming experience (ideally with Python/Jupyter notebooks, git)

References

Choong, M. K., Galgani, F., Dunn, A. G., & Tsafnat, G. (2014). Automatic evidence retrieval for systematic reviews. Journal of Nedical Internet Research, 16(10), e3369.

Herlocker, J. L., Konstan, J. A., Terveen, L. G., & Riedl, J. T. (2004). Evaluating collaborative filtering recommender systems. ACM Transactions on Information Systems (TOIS), 22(1), 5-53.

Prester, J., Wagner, G., Schryen, G., & Hassan, N. R. (2021). Classifying the ideational impact of information systems review articles: A content-enriched deep learning approach. Decision Support Systems, 140, 113432.

Wagner, G., Prester, J., & Paré, G. (2021). Exploring the boundaries and processes of digital platforms for knowledge work: A review of information systems research. The Journal of Strategic Information Systems, 30(4), 101694.

Webster, J., & Watson, R. T. (2002). Analyzing the past to prepare for the future: Writing a literature review. MIS Quarterly, 26(2), xiii-xxiii.

-->
