---
title: "Multi-Agent Vulcan: An Information-Driven Multi-Agent Path Finding Approach" 
collection: publications
permalink: /publication/2024-09-19-multi-agent-vulcan-an-information-driven-multi-agent-path-finding-approach
date: 2024-09-19
venue: 'IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Oral Pitch'
venue_short: 'IROS 2024'
pub_type: conference
authors:
  - Jake Olkin*
  - Viraj Parimi*
  - Brian C. Williams
summary: "Plans paths for multi-robot exploration that maximize the information the team gathers, with distributed coordination that tolerates intermittent communication."
links:
  - label: Paper
    url: https://doi.org/10.1109/IROS58592.2024.10801571
    icon: file-pdf
    btn_class: btn--primary
  - label: arXiv
    page_only: true
    url: https://arxiv.org/abs/2409.13065
    icon: file-pdf
  - label: Code
    url: https://github.com/virajparimi/info-mapf
    icon: code
  - label: Website
    url: https://info-mapf-mers.csail.mit.edu/
    icon: globe
  - label: Video
    page_only: true
    url: https://info-mapf-mers.csail.mit.edu/static/videos/IROS_Oral_Pitch.mp4
    icon: file-video
  - label: Poster
    page_only: true
    url: https://info-mapf-mers.csail.mit.edu/static/files/IROS_Poster.pdf
    icon: file-image
abstract: |-
  Scientists often search for phenomenon of interest while exploring new environments. Autonomous vehicles are deployed to explore such areas where human-operated vehicles would be costly or dangerous. Online control of autonomous vehicles for information-gathering is called adaptive sampling and can be framed as a Partially Observable Markov Decision Process (POMDPs) that uses information gain as its principal objective. While prior work focuses largely on single-agent scenarios, this paper confronts challenges unique to multi-agent adaptive sampling, such as avoiding redundant observations, preventing vehicle collision, and facilitating path planning under limited communication. We start with Multi-Agent Path Finding (MAPF) methods, which address collision avoidance by decomposing the multi-agent path planning problem into a series of single-agent path planning problems. We present an extension to these methods called information-driven MAPF which addresses multi-agent information gain under limited communication. First, we introduce an admissible heuristic that relaxes mutual information gain to an additive function that can be evaluated as a set of independent single agent path planning problems. Second, we extend our approach to a distributed system that is robust to limited communication. When all agents are in range, the group plans jointly to maximize information. When some agents move out of range, communicating subgroups are formed and the subgroups plan independently. Since redundant observations are less likely when vehicles are far apart, this approach only incurs a small loss in information gain, resulting in an approach that gracefully transitions from full to partial communication. We evaluate our method against other adaptive sampling strategies across various scenarios, including real-world robotic applications. Our method was able to locate up to 200% more unique phenomena in certain scenarios, and each agent located its first unique phenomenon faster by up to 50%.
bibtex: |-
  @inproceedings{olkin2024vulcan,
    title     = {Multi-Agent {Vulcan}: An Information-Driven Multi-Agent Path Finding Approach},
    author    = {Olkin, Jake and Parimi, Viraj and Williams, Brian C.},
    booktitle = {Proceedings of the IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
    pages     = {10253--10259},
    year      = {2024},
    doi       = {10.1109/IROS58592.2024.10801571}
  }
header:
  teaser: Info_MAPF_teaser.jpg
  teaser_alt: "Two TurtleBots in a LEGO maze next to the belief map of where targets are"
lead_video: /images/highlights/vulcan.mp4
lead_video_poster: /images/highlights/vulcan.jpg
lead_video_alt: "Two TurtleBots searching a maze, first with an MCTS-based planner and then with Multi-Agent Vulcan"
lead_video_caption: "Two TurtleBots search a maze for targets, first with an MCTS-based planner and then with Multi-Agent Vulcan. The MCTS planner finds 2 targets and Multi-Agent Vulcan finds 5."
---

Robots that explore for phenomena of interest need to avoid redundant observations and collisions, and to keep planning when they lose contact with each other. Multi-Agent Vulcan builds on MAPF with an admissible heuristic that relaxes the team's information gain into a sum over single-robot planning problems. When robots move out of communication range, the team splits into subgroups that plan on their own, which costs little information because robots far apart rarely make redundant observations. In some scenarios it **finds up to 200% more unique phenomena** than other adaptive sampling strategies.
