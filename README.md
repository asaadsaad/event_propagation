### Event Propagation

The propagation is bidirectional, from the window to the event target and back. This propagation can be divided into three phases:

*   From the window to the event target parent: this is the capture phase
*   The event target itself: this is the target phase
*   From the event target parent back to the window: the bubble phase

The event propagation can be stopped in any listener by invoking the stopPropagation method of the event object. This means that all the listeners registered on the nodes on the propagation path that follow the current target will not be called. Instead, all the other remaining listeners attached on the current target will still receive the event.
