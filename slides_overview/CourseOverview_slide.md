\documentclass[10pt, xcolor=dvipsnames]{beamer}
\usetheme{Madrid}
\usecolortheme{seahorse}

% Required packages
\usepackage{tikz}
\usetikzlibrary{shapes, arrows, positioning, calc, decorations.pathreplacing}
\usepackage{graphicx}
\usepackage{booktabs}
\usepackage{ragged2e}
\usepackage{hyperref}
\usepackage{listings}

% Custom colors
\definecolor{pennblue}{RGB}{1,31,91}
\definecolor{pennred}{RGB}{152,30,50}
\setbeamercolor{title}{fg=pennblue}
\setbeamercolor{frametitle}{fg=pennblue}
\setbeamercolor{structure}{fg=pennblue}

% Title page info
\title[Course Overview]{Technology Commercialization}
\subtitle{From Idea to Market}
\author[K. Wang]{Kate Wang}
\institute[Penn State]{
  Penn State University
}
\date{Spring 2025}

% Remove navigation symbols
\setbeamertemplate{navigation symbols}{}

% Custom itemize
\setbeamertemplate{itemize items}[circle]
\setbeamertemplate{enumerate items}[default]

\begin{document}

% Title slide
\begin{frame}
  \titlepage
  \centering

\end{frame}

% About Me
\section{About Me}
\begin{frame}{Let's Warm Up}

    \begin{itemize}
      \item Engineer and math background
      \item 6 years in Los Angeles researching technologies and entrepreneurship
      \item Coach for Nittany AI challenges (e.g., Bytehealth)
    \end{itemize}
    

\end{frame}

\begin{frame}{Your Turn}

    \begin{itemize}
      \item What do you prefer to be called?
      \item Where are you from?
      \item What is your major?
    \end{itemize}
    

\end{frame}


% Course Introduction
\section{Course Overview}

% Facebook vs MySpace Story
\section{Case Study}
\begin{frame}{The Facebook vs. MySpace Story}
  \centering
  \begin{tikzpicture}[
      platform/.style={rectangle, draw, rounded corners, minimum width=3cm, minimum height=1.5cm, align=center, font=\small},
      arrow/.style={->, >=stealth, thick}
    ]
    % Platforms
    \node[platform, fill=blue!20] (fb) at (0,0) {Facebook \\ \footnotesize (Clean Design)};
    \node[platform, fill=red!20] (ms) at (8,0) {MySpace \\ \footnotesize (Customizable)};
    
    % Arrows
    \draw[arrow, bend left=30] (fb) to node[above] {Different Approaches} (ms);
    \draw[arrow, bend left=30] (ms) to node[below] {Same Goal} (fb);
    
    % Outcomes
    \node[below=1.5cm of fb] {\$1T+ Valuation};
    \node[below=1.5cm of ms] {\$580M Acquisition};
  \end{tikzpicture}
\end{frame}

\begin{frame}{Illustration of Facebook vs MySpace}
\includegraphics[width=\textwidth]{facebook_vs_myspace.png}
\end{frame}


\begin{frame}{Key Differences in Execution}
  \begin{columns}
    \column{0.5\textwidth}
    \begin{block}{MySpace}
      \begin{itemize}
        \item Complete profile customization
        \item Top 8 friends
        \item Cluttered ads
        \item No real-name policy
      \end{itemize}
    \end{block}
    
    \column{0.5\textwidth}
    \begin{block}{Facebook}
      \begin{itemize}
        \item Clean, uniform design
        \item Real names only
        \item Targeted advertising
        \item Platform for apps
      \end{itemize}
    \end{block}
  \end{columns}
  
  \vspace{1cm}
  \centering
  \textbf{Lesson:} Execution $>$ Idea
\end{frame}


\begin{frame}{Course Objectives}
  \begin{block}{What We'll Cover}
    \begin{itemize}
      \item Market strategies for technology commercialization
      \item Value creation and capture
      \item Business model development
      \item Case studies of successful (and failed) tech ventures
    \end{itemize}
  \end{block}
  
  \begin{alertblock}{What This Course Is Not}
    \begin{itemize}
      \item Idea generation workshop
      \item Technical R\&D management
      \item IT operations
    \end{itemize}
  \end{alertblock}
\end{frame}


\begin{frame}{Commercialization Tunnel}
\includegraphics[width=\textwidth]{CommercializationTunnel.png}
\end{frame}


% Assignments
\section{Course Components}
\begin{frame}{Assignments and Grading}


      \begin{itemize}
        \item Pre-class blog and discussion (30\%)
        \item In-class participation: Simulation (30\%)
        \item Team project (40\%)
      \end{itemize}

    

\end{frame}

% Pre class blog posting
\begin{frame}{Pre-class blog and discussion}

    \begin{itemize}
      \item Form teams of 3-4 students
      \item Each team is responsible to write a blog for one class session to lead pre-class discussion on canvas
      \item Students that are not part of the blogging team will post comment to join the discussion on canvas

    \end{itemize}
    

\end{frame}

% Simulation
\begin{frame}{Business Simulation}
  \centering
  \textbf{Simulation:} Demand-driven vs. Technology-driven approaches
$https://bcs.statherian.com$
  
\end{frame}
% Team Project
\begin{frame}{Team Project: Website Development}
  \begin{columns}
    \column{0.6\textwidth}
    \begin{itemize}
      \item Form teams of 3-4 students
      \item Develop a business website
      \item Present your technology commercialization plan
      \item Peer evaluations
    \end{itemize}
    
    \column{0.4\textwidth}
    \begin{tikzpicture}
      \node[draw, rectangle, rounded corners, fill=blue!20, minimum width=3cm, minimum height=2cm] (web) {Commercialize picked patent};
      \foreach \i in {1,...,5} {
        \node[draw, circle, fill=red!20] (user\i) at (360/5*\i:2.5cm) {};
        \draw[->] (user\i) -- (web);
      }
    \end{tikzpicture}
  \end{columns}
\end{frame}


% Next Steps
\begin{frame}{This week and next week}


\begin{itemize}

      \item Form project teams
      \item Set up team website
      \item Complete pre-class reading
      \item Prepare for simulation
    \end{itemize}
  

\end{frame}

% Final Slide
\begin{frame}{Key takeaways}
  \centering
  \Huge\textbf{Remember:} Great execution turns good ideas into great businesses!
\end{frame}

\end{document}