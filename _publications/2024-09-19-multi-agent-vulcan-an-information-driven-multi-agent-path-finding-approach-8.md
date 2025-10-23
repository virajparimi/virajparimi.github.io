---
title: "Multi-Agent Vulcan: An Information-Driven Multi-Agent Path Finding Approach" 
collection: publications
permalink: /publication/2024-09-19-multi-agent-vulcan-an-information-driven-multi-agent-path-finding-approach
date: 2024-09-19
venue: 'IROS'
pub_type: conference
authors:
  - Jake Olkin*
  - Viraj Parimi*
  - Brian C. Williams
summary: "Extended MAPF with an information-driven heuristic and distributed coordination so multi-robot explorers maximize unique observations even under intermittent communication."
links:
  - label: Paper
    url: /files/paper8.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Website
    url: https://info-mapf-mers.csail.mit.edu/
    icon: globe
project_links:
  - label: Project Site
    url: https://info-mapf-mers.csail.mit.edu/
abstract: |-
  Scientists often search for phenomenon of interest while exploring new environments. Autonomous vehicles are deployed to explore such areas where human-operated vehicles would be costly or dangerous. Online control of autonomous vehicles for information-gathering is called adaptive sampling and can be framed as a Partially Observable Markov Decision Process (POMDPs) that uses information gain as its principal objective. While prior work focuses largely on single-agent scenarios, this paper confronts challenges unique to multi-agent adaptive sampling, such as avoiding redundant observations, preventing vehicle collision, and facilitating path planning under limited communication. We start with Multi-Agent Path Finding (MAPF) methods, which address collision avoidance by decomposing the multi-agent path planning problem into a series of single-agent path planning problems. We present an extension to these methods called information-driven MAPF which addresses multi-agent information gain under limited communication. First, we introduce an admissible heuristic that relaxes mutual information gain to an additive function that can be evaluated as a set of independent single agent path planning problems. Second, we extend our approach to a distributed system that is robust to limited communication. When all agents are in range, the group plans jointly to maximize information. When some agents move out of range, communicating subgroups are formed and the subgroups plan independently. Since redundant observations are less likely when vehicles are far apart, this approach only incurs a small loss in information gain, resulting in an approach that gracefully transitions from full to partial communication. We evaluate our method against other adaptive sampling strategies across various scenarios, including real-world robotic applications. Our method was able to locate up to 200% more unique phenomena in certain scenarios, and each agent located its first unique phenomenon faster by up to 50%.
bibtex: |- 
  @INPROCEEDINGS{10801571,
    author={Olkin, Jake and Parimi, Viraj and Williams, Brian},
    booktitle={2024 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)}, 
    title={Multi-Agent Vulcan: An Information-Driven Multi-Agent Path Finding Approach}, 
    year={2024},
    volume={},
    number={},
    pages={10253-10259},
    keywords={Additives;Markov decision processes;Path planning;Collision avoidance;Autonomous vehicles;Mutual information;Intelligent robots},
    doi={10.1109/IROS58592.2024.10801571}
  }
header:
  teaser: Info_MAPF.png
  teaser_alt: "Information-driven multi-agent planning"
lead_image: /images/Info_MAPF.gif
lead_image_alt: "Information-driven multi-agent planning"
---

We introduce admissible information heuristics and a communication-aware decomposition strategy so teams seamlessly move between centralized and decentralized planning regimes.
