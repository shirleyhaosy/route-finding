### route-finding

This project is for MSBD Independent Project: Route Planning for Multiple Robots.

1. map_generation_8x8.ipynb and map_generation_14x14.ipynb: Generated maps. Output: map_8_8_v0.txt and map_14_14_v1.txt. map_8_8_v1.txt is manually modified based on map_8_8_v0.txt.
2. /map_sample: Sample images of maps generated. Included in the project report.
3. .ipynb: notebooks to train and test agents to find routes in given map. To test run, you may need to clone this repository and move the whole gym folder to your Python site_packages folder. (Note: you may need to pip uninstall gym first if you have installed OpenAI Gym previously.)
   - If "once" is in the filename: for the scenario that the process that ends when both agents reach their destination.
   - If "lifelong" is in the filename: for the lifelong scenario
   - If 8x8 in the filename: Runs on the 8x8 gridmap
   - If 14x14 in the filename: Runs on the 14x14 gridmap
   - Suffix method 1/method 2: tells which method is implemented in this .ipynb
  
4. /gym: modified from OpenAI Gym.
   - envs/toy_text/frozen_lake.py:
     - Added a new action "PAUSE" for the agent
     - Added new components Kitty (K), Pet Home (P), and Cat food (C)
   - envs/toy_text/imgs: Add icons for K, P, C. Source of icons:
     - <a href="https://www.flaticon.com/free-icons/cat" title="cat icons">Cat icons created by Marz Gallery - Flaticon</a>
     - <a href="https://www.flaticon.com/free-icons/cat-food" title="cat food icons">Cat food icons created by monkik - Flaticon</a>
     - <a href="https://www.flaticon.com/free-icons/cat" title="cat icons">Cat icons created by Freepik - Flaticon</a>
5. /Plot: Plots of all training statistics of E, K or both with method 1 or 2 on different maps. All the plots are attached in the appendix of project report.
   
6. /Demo/epi_200: GIF visualization of the agents' movements.
  - Demo on 8x8 map with method 1 (left) and method 2 (right) <br><br>
    <img src='/Demo/epi_200/kitty_qlearning-8x8map_once_200_episodes_method_1.gif' width='200'> &nbsp; &nbsp;
    <img src='/Demo/epi_200/kitty_qlearning-8x8map_once_200_episodes_method_2.gif' width='200'>
  - Demo on 14x14 map with method 1 (left) and method 2 (right) <br><br>
    <img src='/Demo/epi_200/kitty_qlearning-14x14map_once_200_episodes_method_1.gif' width='200'> &nbsp; &nbsp;
    <img src='/Demo/epi_200/kitty_qlearning-14x14map_once_200_episodes_method_2.gif' width='200'>
    <br>
  - Demo on 8x8 map in lifelong scenarios with method 1 (left) and method 2 (right) <br><br>
    <img src='/Demo/epi_200/kitty_qlearning-8x8map_lifelong_200_episodes_method_1.gif' width='200'>  &nbsp;  &nbsp;
    <img src='/Demo/epi_200/kitty_qlearning-8x8map_lifelong_200_episodes_method_2.gif' width='200'>
    <br>
  - Demo on 14x14 map in lifelong scenarios with method 1 (left) and method 2 (right) <br><br> 
    <img src='/Demo/epi_200/kitty_qlearning-14x14map_lifelong_200_episodes_method_1.gif' width='200'> &nbsp; &nbsp;
    <img src='/Demo/epi_200/kitty_qlearning-14x14map_lifelong_200_episodes_method_2.gif' width='200'>

7. /RL Practice: Forked and modified from <a href = "https://github.com/dennybritz/reinforcement-learning"> reinforcement-learning repository </a>. Just for my own reference and practice when learning <a href = "https://www.davidsilver.uk/teaching/">David Silver's RL Course</a>. I learned how to program RL algorithm with it and decide to cite it here. Can be ignored as it is not directly related to the project itself.

Please contact me if you have any problems. Thank you.

    
 
