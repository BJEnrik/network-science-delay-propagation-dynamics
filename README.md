%% BioMed_Central_Tex_Template_v1.06
%%                                      %
%  bmc_article.tex            ver: 1.06 %
%                                       %

%%IMPORTANT: do not delete the first line of this template
%%It must be present to enable the BMC Submission system to
%%recognise this template!!

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                                     %%
%%  LaTeX template for BioMed Central  %%
%%     journal article submissions     %%
%%                                     %%
%%          <8 June 2012>              %%
%%                                     %%
%%                                     %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%


%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                                                                 %%
%% For instructions on how to fill out this Tex template           %%
%% document please refer to Readme.html and the instructions for   %%
%% authors page on the biomed central website                      %%
%% http://www.biomedcentral.com/info/authors/                      %%
%%                                                                 %%
%% Please do not use \input{...} to include other tex files.       %%
%% Submit your LaTeX manuscript as one .tex document.              %%
%%                                                                 %%
%% All additional figures and files should be attached             %%
%% separately and not embedded in the \TeX\ document itself.       %%
%%                                                                 %%
%% BioMed Central currently use the MikTex distribution of         %%
%% TeX for Windows) of TeX and LaTeX.  This is available from      %%
%% http://www.miktex.org                                           %%
%%                                                                 %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%%% additional documentclass options:
%  [doublespacing]
%  [linenumbers]   - put the line numbers on margins

%%% loading packages, author definitions

%\documentclass[twocolumn]{bmcart}% uncomment this for twocolumn layout and comment line below
\documentclass{bmcart}

%%% Load packages
%\usepackage{amsthm,amsmath}
%\RequirePackage{natbib}
%\RequirePackage[authoryear]{natbib}% uncomment this for author-year bibliography
%\RequirePackage{hyperref}
\usepackage[utf8]{inputenc} %unicode support
%\usepackage[applemac]{inputenc} %applemac support if unicode package fails
%\usepackage[latin1]{inputenc} %UNIX support if unicode package fails


%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                                             %%
%%  If you wish to display your graphics for   %%
%%  your own use using includegraphic or       %%
%%  includegraphics, then comment out the      %%
%%  following two lines of code.               %%
%%  NB: These line *must* be included when     %%
%%  submitting to BMC.                         %%
%%  All figure files must be submitted as      %%
%%  separate graphics through the BMC          %%
%%  submission process, not included in the    %%
%%  submitted article.                         %%
%%                                             %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
\usepackage{array}
\usepackage{booktabs}
\usepackage{graphicx}
% \def\includegraphic{}
% \def\includegraphics{}



%%% Put your definitions there:
\startlocaldefs
\endlocaldefs


%%% Begin ...
\begin{document}

%%% Start of article front matter
\begin{frontmatter}

\begin{fmbox}
\dochead{MSDS 2023 Network Science Final Paper}

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                                          %%
%% Enter the title of your article here     %%
%%                                          %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\title{Delay Propagation Dynamics and Disruptive Elements in Airline Networks}

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                                          %%
%% Enter the authors here                   %%
%%                                          %%
%% Specify information, if available,       %%
%% in the form:                             %%
%%   <key>={<id1>,<id2>}                    %%
%%   <key>=                                 %%
%% Comment or delete the keys which are     %%
%% not used. Repeat \author command as much %%
%% as required.                             %%
%%                                          %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\author[
   addressref={aff1},                   % id's of addresses, e.g. {aff1,aff2}
   corref={aff1},                       % id of corresponding address, if any
   noteref={n1},                        % id's of article notes, if any
   email={BYepes.MSDS2023@aim.edu}   % email address
]{\inits{BJGY}\fnm{BJ Enrik G.} \snm{Yepes}}
\author[
   addressref={aff1},                   % id's of addresses, e.g. {aff1,aff2}
   noteref={n1},                        % id's of article notes, if any
   email={MMenorca.MSDS2023@aim.edu}   % email address
]{\inits{MLRM}\fnm{Maria Loraine R.} \snm{Menorca}}
\author[
   addressref={aff1},                   % id's of addresses, e.g. {aff1,aff2}
   noteref={n1},                        % id's of article notes, if any
   email={GDelCarmen.MSDS2023@aim.edu}   % email address
]{\inits{GMD}\fnm{Gregory Mark T.} \snm{del Carmen}}
\author[
   addressref={aff1},                   % id's of addresses, e.g. {aff1,aff2}
   email={RBanquerigo.MSDS2023@aim.edu}   % email address
]{\inits{RCEB}\fnm{Rozz Charles E.} \snm{Banquerigo}}

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                                          %%
%% Enter the authors' addresses here        %%
%%                                          %%
%% Repeat \address commands as much as      %%
%% required.                                %%
%%                                          %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\address[id=aff1]{%                           % unique id
  \orgname{Asian Institute of Management}, % university, etc
  \street{123 Paseo de Roxas, Legazpi Village, Makati}, %
  \postcode{1229}                                % post or zip code
  \city{Metro Manila},                              % city
  \cny{Philippines}                                    % country
}

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                                          %%
%% Enter short notes here                   %%
%%                                          %%
%% Short notes will be after addresses      %%
%% on first page.                           %%
%%                                          %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\begin{artnotes}
%\note{Sample of title note}     % note to the article
\note[id=n1]{Equal Contributor} % note, connected to author
\end{artnotes}

\end{fmbox}% comment this for two column layout

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                                          %%
%% The Abstract begins here                 %%
%%                                          %%
%% Please refer to the Instructions for     %%
%% authors on http://www.biomedcentral.com  %%
%% and include the section headings         %%
%% accordingly for your article type.       %%
%%                                          %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\begin{abstractbox}

\begin{abstract}
In the complex airline industry, disruptions often trigger chain reactions across transportation systems, leading to delay propagation. This study applies network science, experimenting with Chauhan et al.'s methodologies using the United Airlines network, to address this challenge. It analyzes airport-airport and flight flight connection networks using centrality measures, diameter, percolation, and Chauhan et al.'s priority ranking system.

The purpose of this experiment is to identify disruptive elements, either an airport or a flight, within an airline network, further enhancing the capability to optimize flight operations. Findings reveal a hub-and-spoke topology with major airports as hubs and smaller ones as endpoints, observed in most scale-free, real-world systems. Prioritization identifies Priority 1 elements like DEN and ORD for urgent attention, with Priority 2 and 3 elements (e.g., MCO, ABQ, and GUM) also requiring focus. Notably, flights themselves may not be primary disruptors, but multiple EWR flights hint at operational issues.

The study introduces search radius adjustments as a flexible strategy for airlines to fine-tune disruption mitigation, balancing cost, and effectiveness. This network analysis serves as a guide to making the air transport system resilient against delay propagation and operational disruptions within the intricate airline industry network.
\end{abstract}

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                                          %%
%% The keywords begin here                  %%
%%                                          %%
%% Put each keyword in separate \kwd{}.     %%
%%                                          %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\begin{keyword}
\kwd{airline}
\kwd{delays}
\kwd{disruption}
\kwd{resilience}
\end{keyword}

% MSC classifications codes, if any
%\begin{keyword}[class=AMS]
%\kwd[Primary ]{}
%\kwd{}
%\kwd[; secondary ]{}
%\end{keyword}

\end{abstractbox}
%
%\end{fmbox}% uncomment this for twcolumn layout

\end{frontmatter}

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                                          %%
%% The Main Body begins here                %%
%%                                          %%
%% Please refer to the instructions for     %%
%% authors on:                              %%
%% http://www.biomedcentral.com/info/authors%%
%% and include the section headings         %%
%% accordingly for your article type.       %%
%%                                          %%
%% See the Results and Discussion section   %%
%% for details on how to create sub-sections%%
%%                                          %%
%% use \cite{...} to cite references        %%
%%  \cite{koon} and                         %%
%%  \cite{oreg,khar,zvai,xjon,schn,pond}    %%
%%  \nocite{smith,marg,hunn,advi,koha,mouse}%%
%%                                          %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%%%%%%%%%%%%%%%%%%%%%%%%% start of article main body
% <put your article body there>

%%%%%%%%%%%%%%%%
%% Background %%
%%
\section*{Introduction}

Disruptions in the airline industry can have wide-ranging effects on both the regional and operational aspects of a given area. These disruptions can directly or indirectly impact various crucial sectors, such as tourism, trade, and the overall economy. Flight delays, from a practical standpoint, can significantly influence an airline's management strategy, affecting its reputation, brand, and customer relationships. Consequently, understanding flight operation performance and optimizing ground processes are essential considerations for the airline industry to enhance air traffic management \cite{ref:eurocontrol} and build trust with their customers.

 These disruptions often stem from three primary sources: airlines, airports, and weather conditions. Airlines can contribute to operational hiccups through delays in boarding and disembarkation, longer turnaround times for necessary repairs, and crew shortages. Meanwhile, airports can complicate operations with lengthy security checks and occasional unexpected closures. These closures are often due to weather-related disturbances like tropical cyclones and snowstorms, which affected more than 2,500 flights in 2022 \cite{ref:chauhan}. In 2017, approximately one in five flights in Europe experienced delays of at least fifteen minutes due to various disruptions, accounting for 30\% to 60\% of delays at European airports \cite{ref:eurocontrol, ref:flightdelays}. These delays cost airlines approximately USD 74.20 per minute, resulting in monthly losses exceeding USD 8 million \cite{ref:flightdelays}. Therefore, optimizing these factors to reduce delays can lead to substantial cost savings for the airline industry, which can then be allocated to other important and productive areas.

 Given the intricate nature of the airline industry as a complex distributed transportation system, delay propagation and related issues are a common occurrence. A disruption in one aspect of the transportation system, such as passengers, crew, airports, or airlines, can trigger a chain reaction of problems that affect one element after another. This ripple effect, known as delay propagation \cite{ref:chauhan}, raises the question: in a complex distributed transportation network, how can network science be applied to address delay propagation issues that originate from one element or factor and affect others?

\subsection*{Significance of the Study}
The surge in traveler numbers both before and after the pandemic emphasizes the role of the tourism sector, which is linked to the operations of the airline industry. In the Philippines, for instance, there has been a increase in passenger traffic at airports as people travel to both domestic and international destinations. However, this surge has been accompanied by disruptions, including flight cancellations, diversions, immigration clearance issues, and various other disruptive factors. The situation has even prompted a Senate inquiry \cite{ref:manabat} into these delays and cancellations, highlighting the frustration of passengers and putting pressure on local airlines and airports to enhance their operational efficiency. This scenario is not unique to the Philippines; major airlines worldwide grapple with similar challenges influenced by factors such as adverse weather conditions \cite{ref:bevege} and airport control issues \cite{ref:slow}.

This study follows an approach that employs network analysis concepts to investigate delay propagation within the airline industry systems. The primary goal is to pinpoint the key disruptive elements in the complex airline industry operations. By identifying and understanding these disruptive elements, the airline industry can strategically allocate resources and prioritize areas for improvement. This, in turn, can lead to more streamlined flight operations and the effective mitigation of delays—a benefit that extends to all stakeholders involved.

\subsection*{Brief Discussion of Related Works}
This study builds upon established methodologies introduced by Chauhan et al \cite{ref:chauhan}, who characterized the intricate airline transportation system as a network, with airports serving as nodes and flights as edges \cite{ref:lordan, ref:wang}. These related studies share a common theme, focused on the identification of critical nodes within networks to gain insights into their profound impact on the entire system. Additionally, they delve into the fusion of various concepts, such as network science and techniques, with elements inherent to the airline industry, including dynamic configurations \cite{ref:reggiani}, flight operations \cite{ref:lordan}, historical data analysis, and schedule modeling \cite{ref:chauhan}.

Chauhan et al. \cite{ref:chauhan} laid the foundation for this study by exploring the airline network. Lordan and Sallan \cite{ref:lordan} and Wang et al. \cite{ref:wang} contributed by emphasizing the role of airports as significant nodes in such network. These studies collectively highlighted further the significance of recognizing central nodes for the holistic understanding of network dynamics.

Furthermore, the synergy between network science techniques and the complexities of the airline industry is a recurrent theme in these investigations. Reggiani et al. \cite{ref:reggiani} highlighted the importance of considering dynamic configurations, while Lordan and Sallan \cite{ref:lordan} considered flight operations. Meanwhile, Chauhan et al. \cite{ref:chauhan} utilized historical data and schedule modeling to dissect network behaviors.

\subsection*{Experimental Design}
As previously mentioned, this study follows the methodologies outlined by Chauhan et al. \cite{ref:chauhan}, specifically focusing on airport-airline network modeling, the application of network science techniques—primarily centrality, diameter, and percolation—and a comparative analysis employing Chauhan et al.'s ranking system \cite{ref:chauhan}. This ranking system is employed to identify overlaps between actual disruptive elements in the context of the delay network model and potential disruptive elements within the connection model.

However, one notable constraint is that this study does not explore other network science techniques presented in Chauhan et al. \cite{ref:chauhan} such as density. Instead, our focus remains on the initial four network models and approaches outlined in the reference. This involves investigating combinations of two models (airport-flight and flight connections) and two network types (connection network and delay network), with the exclusion of the more complex multi-layer network type from our analysis.

%\cite{koon,oreg,khar,zvai,xjon,schn,pond,smith,marg,hunn,advi,koha,mouse}

\section*{Data}
The study used Marketing Carrier On-Time Performance data including flight-related information, airport origin and destination details, cancellation status, and departure and arrival times. For a more focused analysis, only data pertaining to United Airlines and flights operating within the United States from May to July 2022 were considered.

In constructing the flight connection network model, we categorize connecting flights as infrequent if they average two or fewer occurrences per week for a specific airport. As for the delay network type, we define delays as instances where flights were delayed by 15 minutes or more, adhering to the industry-standard definition.


\section*{Methodology}
Network analysis is used to effectively study delay propagation and disruptive elements in the aviation industry. In this approach, elements are denoted as nodes (or vertices) $N$ and a set of edges (or links) $E$ is formed among them to reflect their interactions or relationships. For example, consider the concept of an airport-flight (AF) network \cite{ref:chauhan}, where airports are represented as nodes, and a connection is established between two nodes if there exists a flight connecting those airports. Another variant is a flight-flight (FC) network, where flights are treated as nodes, and connections are established when two flights share common passengers and aircraft. Networks can be directed \cite{ref:networktype} such that the edge between nodes carry a specific directionality, or they can be undirected otherwise.

\subsection*{Building the Network}
Taking inspiration from the work of Chauhan et al. \cite{ref:chauhan} that focuses on the identification of disruptive elements within airline networks, this study also explored two network models: the Connection Network (CN) and the Delay Network (DN).

CN models an airline’s schedule using shared information among flights such as passengers, crew, and aircraft tail numbers. It considers the scheduled arrival and departure times, as well as the origin and destination airports to identify potentially disruptive elements in the network. On the other hand, DN makes use of an airline’s historical operational data, serving as a specific subset of CN. It focuses on actual disruptive elements such as delayed flights and their connections, which may trigger delay propagation within the system.

Considering the two network models, CN and DN, along with the two variations, AF and FC, we arrive at a total of four distinct networks: AFCN, AFDN, FCCN, and FCDN, as outlined in Table \ref{tab:networkmodels}.


\begin{table}[h!]
\centering
\caption{Summary of different network models referenced from Chauhan et. al's work \cite{ref:chauhan}.}
    \label{tab:networkmodels}
    \begin{tabular}{m{1cm} m{1cm} m{2.8cm} m{2.8cm} m{2.8cm}}
        \toprule
        Network & Node & Link & Link Weight & Purpose \\ \hline
        AFCN & Airports & At least one flight between airports & Flight frequency & Analyze airline schedules.\\
        AFDN & Airports & At least one delayed flight between airports & Delayed flight frequency & Analyze historical airline operations data.\\
        FCCN & Flights  & Shared flight connection  & Flight connection frequency & Analyze flight schedules. \\
        FCDN & Flights  & Shared delayed flight connection  & Delayed flight connection frequency & Analyze historical flight operations data. \\
        \bottomrule
    \end{tabular}
\end{table}


\subsubsection*{Airport-Flight Connection Network (AFCN)}
AFCN is a directed network, with its nodes representing the origin and destination airports. A link is made between two airports if there exists at least one flight connecting them, and the weight of this connection is determined by the number of flights operating between the respective airports. This network configuration can be used to identify potentially disruptive airports or airport pairs, as it is based on the level of traffic between them.

\subsubsection*{Airport-Flight Delay Network (AFDN)}
AFDN shares similarities with AFCN, but with a more focused perspective. This network exclusively considers delayed flights when establishing links and determining their weights. This approach aids in pinpointing airports that have historically played a role in disrupting airline operations.

\subsubsection*{Flight-Flight Connection Network (FCCN)}
FCCN is another directed network within our study. In this configuration, individual flights are considered as nodes, and a link is established when two flights share a connection. In this context, a “flight connection” is defined as having shared passengers, crew members, or aircraft tails. This approach allows us to identify potential disruptive flights and flight connections that have the capacity to impact other flights within the network.

\subsubsection*{Flight-Flight Delay Network (FCDN)}
FCDN resembles FCCN, but it focuses solely on delayed flights as nodes and flight connections associated with delay propagation. This perspective looks at flights and their connections that have a history of causing delays within the network.

\subsection*{Characterizing the Network}
The analysis of topological properties within the four networks defined previously helps in identifying critical nodes and the formulating strategies for designing a more efficient and resilient airline network. This understanding of the network's structural strengths and weaknesses serves as a guide for addressing vulnerabilities to improve the network's capacity to withstand disruptions and ensuring a more reliable airline operation.

The network properties analyzed in this work include degree distribution, diameter, and centrality measures. Percolation is also one of the techniques used to understand and describe disruptive elements in the network.

The degree \cite{ref:degree}, $k$, is one of the fundamental properties of a node in a network, indicating the number of links it has with other nodes. In the context of a directed network, such as an airport-flight connection, the degree can be further categorized into two types: (1) in-degree, $k_{in}$, representing the count of incoming edges that converge at a node, and (2) out-degree, $k_{out}$, denoting the tally of outgoing edges originating from a node.

Degree distribution, $p_k$, characterizes the probability that a randomly selected node within the network has a degree of $k$, as shown in Equation \ref{eq:degdist}. The study of degree distributions gives an insight to the underlying mechanisms of how nodes form connections or the network’s topological structure. Moreover, it allows the identification of hubs, a crucial aspect in the context of airline networks, and their potential role in either alleviating or propagating delays.
\begin{eqnarray}\label{eq:degdist}
    p_k = \frac{N_k}{N}
\end{eqnarray}
where $N$ is the total number of nodes in the network, and $N_k$ is the number of nodes with degree $k$.

The diameter, $D$ (Equation \ref{eq:diameter}) of a connected network \cite{ref:chauhan} is the maximum shortest distance between any two nodes within that network. In cases where the network is disconnected, this value becomes infinite, signifying that certain nodes cannot be reached \cite{ref:desilva}. This metric is used to determine the minimal number of flights needed to propagate delays across the entire network. While a smaller diameter indicates a higher level of connectivity within the air transport network, it also has a potential downside. Specifically, a smaller diameter may also imply increased vulnerability to delays, as it would require only a few flights to propagate delays and disrupt the entire network.
\begin{eqnarray}\label{eq:diameter}
    D = \mathrm{max}(l_{ij})
\end{eqnarray}
where $l_{ij}$ is the path length or distance between nodes $i$ and $j$.

Centrality measures quantify the significance of nodes within a network. In this study, two measures are considered – out-degree centrality and betweenness centrality.

Out-degree centrality [1] (Equation \ref{eq:outdegcent}) assigns importance to nodes that have a substantial number of outgoing edges. As an example, in flight-flight networks, high out-degree centrality indicates that delays in well-connected flights may have a cascading effect on other flights within the network.
\begin{eqnarray}\label{eq:outdegcent}
    c_D(i) = \frac{k_{out}(i)}{N}
\end{eqnarray}
where $k_{out}(i)$ is the out-degree of node $i$.

Betweenness centrality \cite{ref:betcentrality}, shown in Equation \ref{eq:node_betcent}, measures a node’s ability to act as a bridge, facilitating the flow of information between other nodes. Nodes with higher betweenness centrality are critical in cascading delays since they can reach the entire network with fewer “hops”. For example, if the network has scale-free properties, an airport with high betweenness centrality may serve as a hub connecting multiple airports by sharing flights with them. Consequently, any disruption at this airport, such as a delayed scheduled flight or a shutdown, can exert a greater impact on other airports compared to those with lower betweenness scores.
\begin{eqnarray}\label{eq:node_betcent}
    c_B(n) = \sum_{i,j \in{N}}\frac{\sigma(i,j|n)}{\sigma(i,j)}
\end{eqnarray}
where $\sigma(i, j)$ is the number of shortest paths between all pairs of nodes, and $\sigma(i, j|n)$ is the number of shortest paths between all pairs $(i, j)$ through node $n$. Similarly, the edge betweenness centrality of edge $e$ is given by Equation \ref{eq:edge_betcentrality}.
\begin{eqnarray}\label{eq:edge_betcentrality}
    c_B(e) = \sum_{i,j \in{N}}\frac{\sigma(i,j|e)}{\sigma(i,j)}
\end{eqnarray}

Percolation \cite{ref:li} involves the study of the changes in a network’s structure when nodes or edges are systematically removed. To study which airports or flights require immediate attention to avoid delay propagation or more significant disruptions, the concept of dynamic betweenness centrality \cite{ref:chauhan} was considered. Dynamic betweenness centrality is the recalculated scores within the network after selectively removing nodes with the highest betweenness values.

\subsection*{Identifying and handling disruptive elements}
In this work, disruptive airports and flights are categorized as those with high centrality scores within the network. The pool of potential disruptive elements is drawn from CN, while actual disruptive elements are identified from DN.

Following the ranking system established by Chauhan et al. \cite{ref:chauhan}, the priority levels among the disruptive elements are assessed to identify areas requiring immediate attention for improving airline operations. The highest-priority elements demanding prompt resolution are those that emerge as both potential and actual disruptive elements, and consistently recognized as significant by multiple techniques such as percolation and betweenness centrality. The order of prioritization for other scenarios in this ranking system is presented in Table \ref{tab:rankingsystem}, arranged in descending order of importance.
\begin{table}[h!]
\centering
\caption{Chauhan et al.'s Ranking System for Prioritizing Disruptive Elements within a Network (in decreasing order).}
    \label{tab:rankingsystem}
    \begin{tabular}{m{1.7cm} m{3cm} m{3cm} m{3cm}}
        \toprule
        Priority Level & CN-DN & Techniques & Interpretation  \\ \hline
        1\centering & Potential and actual disruptive elements overlap & Overlapping elements come up in multiple techniques & Schedule disruptions \\
        2\centering & Potential and actual disruptive elements overlap & Overlapping elements come up in only one technique & Schedule issue \\
        3\centering & No overlap between potential and actual disruptive elements  & Some actual disruptive elements come up in multiple techniques  & Operation disruptions \\
        4\centering & No overlap between potential and actual disruptive elements  & No disruptive elements come up in multiple techniques  & No schedule issue \\
        5\centering & No overlap between potential and actual disruptive elements  & Some potential disruptive elements come up in multiple techniques  & Only identifies the busiest elements in the network \\
        \bottomrule
    \end{tabular}
\end{table}


\section*{Results and Discussion}
\subsection*{AC Network}

The scale-free property, as defined in network theory, signifies that a small number of nodes, represented by the hubs, possess a disproportionately large number of connections. In contrast, the majority of nodes, representing airports in this context, maintain only a limited number of connections. This intrinsic feature is a recurring phenomenon observed in various real-world systems, including airport networks.

\begin{figure}[h!]
\centering
\includegraphics[width=0.96\textwidth]{figures/fig_degdist.pdf}
 \caption{Degree Distributions of United Airlines' AFCN (left) and AFDN (right).}
 \label{fig:degdist}
\end{figure}

Conversely, smaller airports, which often serve as endpoints of flight routes, tend to have fewer connections in comparison to their larger counterparts. This discrepancy in connectivity reflects the inherent structure of the network. Figure \ref{fig:degdist} visually represents this concept, highlighting that a significant portion of airports, particularly smaller regional ones, possess only a limited number of direct connections to other airports. In contrast, a select few hubs prominently emerge with their extensive network of connections, emphasizing their indispensable role in shaping the overall transportation network.

This hub-and-spoke structure are observed in both CN and DN. in airport networks is not exclusive to the CN model representing route connectivity. It also manifests a striking resemblance in degree structure within DN.

\begin{figure}[h!]
\centering
\includegraphics[width=0.96\textwidth]{figures/fig_minflight.pdf}
 \caption{Minimum Flights to Propagate Delays Across United Airlines' Networks}
 \label{fig:minflights}
\end{figure}

There is also a similarity in results between AFCN and AFDN in terms of delay propagation dynamics. Both networks have been found to have a matching diameter of four, as shown in Figure \ref{fig:minflights}. This means that, in both cases, it only takes a maximum of four connecting flights to traverse the network between the two most distant airports while following the shortest path.

 Another reason behind the similarity in results, thus far, lies in the shared fundamental characteristics of these networks. The only difference between these types is the consideration of elements, with DN considering flights tagged as delayed. In the context of this study, this similarity means that either CN or DN can be analyzed separately, and results are applicable to either network type.

\subsubsection*{Key Airports}

\begin{figure}[h!]
\centering
\includegraphics[width=0.96\textwidth]{figures/fig_airport_odc.pdf}
 \caption{The Central Hubs: Denver International Airport (DEN) and Chicago O'Hare International Airport (ORD)}
 \label{fig:airport_odc}
\end{figure}

 As illustrated in \ref{fig:airport_odc}, the prominence of Denver International Airport (DEN) and Chicago O'Hare International Airport (ORD) is readily evident. These two airports stand out as central hubs within the network structure.

 Their significance lies in the fact that a substantial number of connecting flights originate from DEN and ORD. Moreover, these airports experience a stark contrast in air traffic volume when compared to other airports in the network. This elevated level of connectivity and traffic volume designates them as the busiest airports in the network.

An intriguing aspect worth noting is that these central airports, characterized by their high out-degree centrality, also fall into the category of disruptive airports. A disruptive airport, in this context, is an airport that, when affected by a delay or disruption, has the potential to propagate these disruptions to other airports in the network. In essence, DEN and ORD play a pivotal role not only in enabling extensive connectivity but also in influencing the network's overall resilience, robustness, and efficiency.

\begin{figure}[h!]
\centering
\includegraphics[width=0.96\textwidth]{figures/fig_airport_bc.pdf}
 \caption{Comparable to Degree Centrality, Yet Distinctive}
 \label{fig:airport_bc}
\end{figure}

 Node betweenness centrality, critical in identifying information flow, presents a different set of influential airports. As shown in Figure \ref{fig:airport_bc}, DEN, ORD, George Bush International Airport (IAH), Newark Liberty International Airport (EWR), and San Francisco International Airport (SFO) are consistently the top five airports with both high out-degree centrality and high betweenness centrality. Note that with the Ranking System, these airports have exhibit overlap in terms of network properties, and can be considered as the most disruptive networks, influencing information flow, delay propagation, and flight operations disruptions.

\begin{figure}[h!]
\centering
\includegraphics[width=0.96\textwidth]{figures/fig_airport_ebc.pdf}
 \caption{Top 10 Airport Connections with the Highest Betweenness Centrality}
 \label{fig:airport_ebc}
\end{figure}

Exploring edge betweenness centrality (Figure \ref{fig:airport_ebc}), on the other hand, gives insights to the critical airport pairings in the network. The airport pairings of Daniel K. Inouye International Airport (HNL)–Antonio B. Won Pat International Airport (GUM), having the the highest edge betweenness centrality, and DEN–IAH being the close second, influence disruptive elements and delay propagation within the network.

\begin{figure}[h!]
\centering
\includegraphics[width=0.96\textwidth]{figures/fig_airport_dynamicbc.pdf}
 \caption{Top 10 Airports with the Highest Dynamic Betweenness Centrality}
 \label{fig:airport_dynamicbc}
\end{figure}

 In terms of percolation, investigating dynamic betweenness centrality of the airports shown in Figure \ref{fig:airport_dynamicbc}, the most critical airport is ORD. Often coming in second behind DEN in previous metrics, ORD emerges as the most influential airport if percolation is considered. This means that when ORD is removed from the network, or in practical terms, has sudden outage, disruption is propagated with the highest probability across the entire network.

\subsection*{FC Network}
Note that the nodes in this network represent individual flights rather than airports, and the edges symbolize the connections between these flights. Notably, in Figure \ref{fig:flight_odc}, a striking observation emerges: there is less node similarity between CN and DN. This discrepancy can be attributed to the vast difference in the volume of nodes compared to that of the Airport Network. 

In contrast to the AC Network, where airports serve as nodes and often exhibit a higher degree of interconnectivity, the FC Network showcases a different pattern. Flights, as nodes, tend to be less interconnected, reflecting that this network type is a more intricate web of flight routes and schedules.

\begin{figure}[h!]
\centering
\includegraphics[width=0.96\textwidth]{figures/fig_flight_odc.pdf}
 \caption{Top 10 Flight Connections with the Highest Out-Degree Centrality}
 \label{fig:flight_odc}
\end{figure}

Despite these differences, a common thread weaves through both the AC and the FC Network—the criticality of EWR. This airport stands out prominently in the context of flights, underscoring its significance as a central hub connecting various flight routes.

\subsubsection*{Key Flights}
Figure \ref{fig:flight_bc} provides a ranking of flight connections for both network types in terms of betweenness centrality. Notably, this reveals distinct disruptive elements in the FC networks. What stands out is the absence of any intersection between the potential disruptive elements in FCCN and the actual disruptive elements in FCDN. The divergence suggests that while certain flights may have the potential to significantly impact network connectivity, real-world disruptions are influenced by a multitude of factors, including delays and operational issues.
\begin{figure}[h!]
\centering
\includegraphics[width=0.96\textwidth]{figures/fig_flight_bc.pdf}
 \caption{Top 10 Flight Connections with the Highest Betweenness Centrality}
 \label{fig:flight_bc}
\end{figure}

Edge Betweenness Centrality in the context of flights may initially appear less intuitive, as the traditional concept of edges between nodes doesn't align seamlessly with individual flights. However, one way to conceptualize it is to consider it as the measure of connectivity between connecting flights. In essence, it gauges the importance of specific flight connections in facilitating the flow of passengers or cargo between different parts of the network.
\begin{figure}[h!]
\centering
\includegraphics[width=0.96\textwidth]{figures/fig_flight_ebc.pdf}
 \caption{Top 10 Flight Connections with the Highest Edge Betweenness Centrality}
 \label{fig:flight_ebc}
\end{figure}

Figure \ref{fig:flight_ebc} provides a ranking of flight connections for both network types in terms of edge betweenness centrality (or the influence in facilitating information flow or, in practical terms, flow of passengers, cargo, etc). A similar pattern as with betweenness centrality is observed – there is minimal to no overlap between the actual disruptive elements and the potential disruptive elements. A recurring observation in this analysis is the frequent occurrence of SFO and EWR. This suggests that these airports play a crucial role in connecting various flights within the network, potentially making them central hubs for passenger and cargo transfers, thus has the highest degree of influence in terms of alleviating or propagating delays and disruptions.

\subsection*{Impact of Removing Disruptive Elements} 

\begin{figure}[h!]
\centering
\includegraphics[width=0.96\textwidth]{figures/fig_flight_dynamicbc.pdf}
 \caption{Top 10 Flight Connections with the Highest Edge Dynamic Betweenness Centrality}
 \label{fig:flight_dynamicbc}
\end{figure}

An intriguing observation in Figure \ref{fig:flight_dynamicbc} surfaces in the course of this percolation study. AFDN exhibits a notable lack of interconnectedness. The root of this lies in the constraint of utilizing only three months' worth of data for the study. Given the opportunity and without the limitations posed by computing capacity, the study could undoubtedly be extended to encompass a more substantial dataset, mitigating the issue of limited interconnectedness.

\begin{table}[h!]
\centering
\caption{Disruptive Airports based on Chauhan et al.'s Ranking System shown in Table \ref{tab:rankingsystem}. Note that no airports were qualified under priority levels 4 and 5.}
\label{tab:disruptive_airports}
    \begin{tabular}{m{3.8cm} m{3.8cm} m{3.8cm}}
        \toprule
        Priority 1 & Priority 2 & Priority 3 \\
        \textit{Schedule disruption} & \textit{Schedule issue} & \textit{Operation disruption} \\
        \midrule
        Denver International Airport (DEN) & Orlando International Airport (MCO) & Antonio B. Won Pat International Airport (GUM) \\
        Chicago O'Hare International Airport (ORD) & Albuquerque International Sunport (ABQ) & \\
        George Bush Intercontinental Airport Houston (IAH) & & \\
        Newark Liberty International Airport (EWR) & & \\
        San Francisco International Airport (SFO) & & \\
        Washington Dulles International Airport (IAD) & & \\
        The Daniel K. Inouye International Airport (HNL) & & \\
        Los Angeles International Airport (LAX) & & \\
        Cleveland Hopkins International Airport (CLE) & & \\
        \bottomrule
    \end{tabular}
\end{table}

Employing Chauhan et al.'s ranking system \cite{ref:chauhan}, Table \ref{tab:disruptive_airports} shows the most disruptive airports given overlaps among the metrics discussed prior. Some of the airports that need to be prioritized are DEN and ORD, as recurrently highest in terms of centrality scores.

\begin{table}[h!]
\centering
\caption{Disruptive Flights based on Chauhan et al.'s Ranking System shown in Table \ref{tab:rankingsystem}. Note that no flights were qualified under priority levels 1 and 2.}
\label{tab:disruptive_flights}
    \begin{tabular}{m{3.8cm} m{3.8cm} m{3.8cm}}
        \toprule
        Priority 3 & Priority 4 & Priority 5 \\
        \textit{Operation disruption} & \textit{No schedule issue} & \textit{Busiest flights} \\
        \midrule
        Flight 1162 01:05 STD BQN-EWR & Flight 1044 07:00 STD MFE-IAH & Flight 2494 14:40 STD IAH-EWR \\
        Flight 1190 18:30 STD EWR-LAX & Flight 1128 07:00 STD SFO-EWR & \\
        Flight 1543 19:57 STD EWR-SJU  & Flight 2606 19:45 STD ORD-LGA & \\
        Flight 1666 23:55 STD SFO-EWR & Flight 2629 06:00 STD LGA-IAH & \\
        Flight 2218 01:05 STD SJU-EWR & & \\
        Flight 2614 12:45 STD LAX-EWR & Flight 2652 13:25 STD SFO-BOS & \\
        Flight 2674 16:50 STD EWR-LAX & Flight 499 14:40 STD BOS-EWR & \\
        Flight 505 23:59 STD SFO-IAH & Flight 715 12:10 STD SAN-IAH & \\
        Flight 569 19:56 STD EWR-BQN & Flight 800 07:00 STD EWR-MCO & \\
        \bottomrule
    \end{tabular}
\end{table}

On the other hand, Table \ref{tab:disruptive_flights} shows the most disruptive flights. Some of the airports that can be highlighted here are EWR, SFO, and LAX, which need to be prioritized in terms of optimizing flight operations, so as to mitigate delays and disruptions.

Note that there is an option to adjust the search radius, which directly influences the sensitivity of the framework's results. A lower limit on the number of disruptive elements signifies a more stringent and budget-constrained approach. In contrast, a higher limit relaxes this constraint but is advisable primarily when an airline possesses the financial capacity to address a larger number of disruptive elements effectively.

\section*{Conclusion}

The analysis of airline networks reveals the prevalence of a hub-and-spoke topology, a hallmark of scale-free networks. This network structure highlights the importance of major airports as hubs, connecting numerous flights, while smaller airports serve as endpoints with fewer connections.

The exploration of disruptive elements within these networks, categorized by priority, highlights further the importance of addressing potential disruptions. Priority 1 elements, exemplified by airports like DEN and ORD, require immediate attention due to their impact on schedule and operations. Priority 2 and 3 elements, such as MCO, ABQ, and GUM, also merit consideration but to a lesser degree.

These findings reveal that flights themselves may not be significant contributors to schedule disruptions or issues within the airline network. However, the presence of multiple EWR flights in Priority 3 suggests a notable operational disruption centered around this airport.

Moreover, the flexibility to adjust the search radius provides airlines with options to fine-tune their disruption mitigation strategies. A lower limit implies a more stringent approach, suitable for budget-conscious airlines, while a higher limit offers a more comprehensive but budget-intensive strategy.

\section*{Recommendations}

\paragraph*{Prioritization of Disruptive Elements} Airlines should prioritize addressing disruptive elements categorized under Priority 1, followed by Priority 2 and Priority 3, as defined by the Chauhan et al. framework. Priority 1 elements, such as Denver International Airport (DEN) and Chicago O'Hare International Airport (ORD), should receive immediate attention due to their significant impact on schedule disruptions and operational issues.

\paragraph*{Operational Disruptions} Airlines should pay particular attention to airports categorized under Priority 3, such as GUM, as they exhibit a significant number of operational disruptions. Multiple occurrences of airports like Newark Liberty International Airport (EWR) in Priority 3 indicate operational challenges that require mitigation strategies.

\paragraph*{Data Collection and Analysis} To better address disruptions, airlines should invest in continuous data collection and analysis. Real-time monitoring of flight connections, airport performance, and network disruptions can enhance decision-making and response strategies.

\paragraph*{Interconnectedness in Delay Networks} In the context of delay networks, efforts should be made to enhance interconnectedness. The observation that the removal of only two nodes can lead to a complete disruption highlights the importance of network robustness. Airlines should explore methods to improve connectivity within delay networks.

\paragraph*{Consider Expanding the Search Radius} The study's search radius was limited to the top 10 disruptive elements per technique. To gain a more comprehensive understanding of disruptive elements, airlines may consider expanding the search radius, especially if budget constraints allow for a broader analysis. This would provide a more nuanced view of potential disruptions within the network.

\paragraph*{Sensitivity Adjustment} Airlines should be mindful of adjusting the sensitivity of the framework results. Lower limitations on disruptive elements provide a stricter approach, suitable for budget-constrained situations. Conversely, higher limitations relax constraints and are advisable when resources are available to address disruptions effectively.

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                                          %%
%% Backmatter begins here                   %%
%%                                          %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\begin{backmatter}

%\section*{Competing interests}
%  The authors declare that they have no competing % interests.

%\section*{Author's contributions}
%    Text for this section \ldots

%\section*{Acknowledgements}
%  Text for this section \ldots

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                  The Bibliography                       %%
%%                                                         %%
%%  Bmc_mathpys.bst  will be used to                       %%
%%  create a .BBL file for submission.                     %%
%%  After submission of the .TEX file,                     %%
%%  you will be prompted to submit your .BBL file.         %%
%%                                                         %%
%%                                                         %%
%%  Note that the displayed Bibliography will not          %%
%%  necessarily be rendered by Latex exactly as specified  %%
%%  in the online Instructions for Authors.                %%
%%                                                         %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

% if your bibliography is in bibtex format, use those commands:
\bibliographystyle{bmc-mathphys} % Style BST file (bmc-mathphys, vancouver, spbasic).
\bibliography{bmc_article}      % Bibliography file (usually '*.bib' )
% for author-year bibliography (bmc-mathphys or spbasic)
% a) write to bib file (bmc-mathphys only)
% @settings{label, options="nameyear"}
% b) uncomment next line
%\nocite{label}

% or include bibliography directly:
% \begin{thebibliography}
% \bibitem{b1}
% \end{thebibliography}


%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%                               %%
%% Figures                       %%
%%                               %%
%% NB: this is for captions and  %%
%% Titles. All graphics must be  %%
%% submitted separately and NOT  %%
%% included in the Tex document  %%
%%                               %%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%%
%% Do not use \listoffigures as most will included as separate files


\end{backmatter}
\end{document}
