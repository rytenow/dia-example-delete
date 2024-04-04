## Week 13
* What is the API class in Babylon.js that allow you to use 360 images as the skybox?  
**Answer:** PhotoDome
* Interaction Mechanics: Viewpoint Control, Hand Gestures, Body Gestures

* What is Embodiment?  
  - Embodiment is perception that a virtual body is one's own, often correlated to Presence
  - Improve tracking fidelity
  - Implement multimodal sensory feedback: visual, auditory, haptic, etc
  - Implement personalization: e.g. Meta's mirror
* Many users tend to route their hands behind the virtual saw blade when asked to place their hands in the target position. Why is the primary reason?  
**Answer:** High embodiment via realistic hand representation and precise tracking
* **Question:** In developing a VR simulation game for urban exploration, players will navigate through a large city environment with a mix of narrow streets and open spaces. The game aims to provide realistic notions of distance and scale, with the ability to explore freely. At the same time, cybersickness should be minimised. Note also that the physical space available for the VR experience is limited.  
  ![Question about VR simulation, what locomotion to use](images/wk13_menti_qn_1.png)  
  **Answer:** :heavy_check_mark: Walking-in-place with HTC Vive HMD and trackers
  :x: Teleportation
  :x: Joystick-based
  :x: Walking-in-place with KatVR 360 sidemill
  :x: Tracking real movement in physical space
* Implementing Interactions
  - Behaviours are predefined, reusable interactions without custom code. Common interactions like drag, scale, follow, etc
  - ActionManager allows you to define property changes triggered by pre-defined events. Able to customise interaction parameters like duration, condition, triggers
  - Observables is a general code construct for observer pattern. It means to subscribe and receive notifications to events. Able to fully customise interactions based on the observed events.
* Coroutines, is a form of parallel programming in javascript.  
  **Question:** What is the order of the console logs?  
  ![Question about order of console.log in async/await](images/wk13_menti_qn_2.png)  
  **Answer:** 2, 3, 4, 1

* **Question 34:** In our VR campus exploration game for the next release, a key focus is to reduce cybersickness. Which is/are suitable implementation approaches?  
  ![Question about order of console.log in async/await](images/wk13_menti_qn_34.png)  
  **Answer:** :heavy_check_mark: Real-walking instead of the current joystick-based locomotion  
  :heavy_check_mark: Reduce the FOV during movement  
  :x: Implement progressively challenging levels  
  :x: Implement GUI elements to present clear goals at each step  
  :x: Increase visual fidelity of the graphics with physically-based shaders  
  :x: Add AI-driven human characters with realistic behaviors
- **Question 35:** Which of the following implementations will this design translate into?
  > A design goal is for users in our VR museum app to have a smooth engaging experience in which they naturally know what to do in each step of the experience.

  **Answer:** :heavy_check_mark: Create gamification features to guide users through the experience  
  :x: Create a walking-in-place locomotion feature  
  :x: Create a teleportation locomotion feature  
  :x: Create high-fidelity realistic 3D museum artifacts  
  :x: Create finger-tracked hand gestures to inspect museum artifacts
- **Question 36:** What data collection methods can be appropriate here?
  > A design goal is for users in our VR museum app to have a smooth engaging experience in which they naturally know what to do in each step of the experience.

  **Answer:** :heavy_check_mark: Let users fill in the FSS (Flow State Scale)  
  :x: Perform semi-structured interviews with users  
  :x: Create telemetry tracking mechanisms to observe users  
  :x: Let users fill in the IPQ (Igroup Presence Questionnaire)  
  :x: Let users fill in the VRSQ (Virtual Reality Sickness Questionnaire)