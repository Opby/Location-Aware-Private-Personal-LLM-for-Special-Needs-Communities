# Introduction
* A Personal Assistant prototype to demonstrate that a LLM hosted on a local device can be used to provide personalized instructions for special needs with accurate location detection powered by UWB proactively:
All user data can stay on local devices for privacy protection: Prove the hypothesis that a small LLM model with 2B parameters can be deployed and run on a typical local device with acceptable latency.
Fine tuned smaller LLB can achieve similar quality as larger LLMs for specific tasks: Fine tuned 2B LLM can provide personalized pace, length of sentences and structure to better serve special needs communities. 
UWB can be used to proactively trigger conversation with a user based location: Implement an end-to-end UWB triggered workflow sending prompts to the LLM to guide the user for routine daily tasks.

# System Architecture and User Flow Chart
* Location Detection Layer: Personal assistant will actively detect user’s location and proactively trigger location base conversation, e.g. help user brush teeth if user is in bathroom. This layer will involve UWB hardware as the mechanism for location detection
* Text/Speech Conversion Layer: A local text-speech conversion engine is used to serve as the communication interface between user and LLM
 * LLM Layer: A fine tuned LLM is running on a local device as a service to generate real-time response based on the prompt that is generated based on the user’s location and response.<img width="1021" alt="Screen Shot 2025-04-05 at 2 11 23 PM" src="https://github.com/user-attachments/assets/55a1f425-965a-49c6-ba49-f6ddcafd317a" />

 # System Demo
 * A use case is selected for demo
When the user gets in the bathroom in the morning, LLM will ask if they need help brushing teeth and washing face and provide instructions tailored for the user with personalized pace. 
<img width="795" alt="Screen Shot 2025-04-05 at 2 13 25 PM" src="https://github.com/user-attachments/assets/7632c636-fecc-4367-9a8b-36fe33432619" />

 # Software code
 * We implemented complete end to end user flow to demonstrate a location-triggered conversation between LLM and user
All data flow are local, i.e. , absolutely no data uploaded to any servers to fully protect user privacy and optimize for cost and latency

* Please check the repo for python code
