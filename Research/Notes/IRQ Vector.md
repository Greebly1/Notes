
A logical/virtual representation of a [[IRQ Line]]

A logical interrupt will be given a number that can be used by the interrupt controller to determine which device created the interrupt,
	but more importantly, the IRQ vector is used to pick the correct [[Interrupt Service Routine]] 

In logical interrupt systems a [[Interrupt Request]] will be accompanied by its IRQ vector. 