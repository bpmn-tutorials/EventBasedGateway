Project for quick testing of Event Gateways
=======================

This project contains two processes to test Event Gateways.

#### EventGatewayTest.bpmn
Contanis Event Gateway and all 4 possible outgoing events:
* Timer
* Signal
* Message
* Condition

##### Timer
To test Timer event just wait 30 seconds and this event will fire automatically.

##### Signal
Send `someSignal` to a running instance of a process to execute signal event branch.

##### Message
Send `Message-someMessage` to a running instance of a process to execute message event branch.

##### Condition
To test this branch, use the second process attached to this project. Condition is configured to execute branch in case `Person` object with name equals to `Ivan` will be added to the kie base. To do so, execute AddToKieBase.bpmn and set `Ivan` as a name for a new person in kie base.
