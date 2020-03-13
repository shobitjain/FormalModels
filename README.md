# FormalModels
iUML-B and UTA models



# Overview of Case Study
In order to demonstrate the CCD methodology with integrated formal methods, we use an airport control system example. We propose this case study for presenting the verification of behavioral and timing properties by combining two complementing formalisms Event-B and UTA. We focus only on the landing control with one runway. Based on system requirements, we have two types of landing, namely, emergency landing and normal landing. The flight control is in charge of safe landing by giving airplanes permission to land at appropriate times. For normal landing planes may queue up to enter the landing runway. There are two queues with different priorities based on the planes fuel level. An
emergency landing has higher priority than both queues. In case of an emergency landing, no other plane can land and all landing requests are rejected. Only one emergency landing can take place at a time. As a safety requirement it is ensured that there is no plane in the runway before allowing another plane to use it.

The model of the airport system consists of one abstract model with three refinement steps. The abstract model presents the general view of the airport system, with two landing modes. In the first refinement step, we introduce two queues with different priorities for normal landing. Next, we implement the FIFO policy of the queues. In the last refinement step, we introduce fuel level for each plane.
