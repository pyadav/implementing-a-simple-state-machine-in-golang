# Basic State Machine in Golang

This repository contains an implementation of a basic state machine in Go.

## Description
A state machine is a mathematical model that describes the behavior of a system based on a set of states and the transitions between those states. This implementation demonstrates a simple traffic light system with three states: red, yellow, and green. Each transition is triggered by an event, such as a timer running out or a sensor detecting a car at an intersection.

## Usage
To use the state machine, simply create an instance of the StateMachine struct with the desired initial state and call the Transition method in a loop to simulate the system's behavior.
```go
func main() {
  sm := NewStateMachine(&GreenLight{})

	for {
		sm.Transition()
	}
}
```

1. Clone the repository to your local machine.
2. Run the server using the go run command:

```bash
# clone the repo
git clone git@github.com:pyadav/implementing-a-simple-state-machine-in-golang.git
go run main.go
```
## License

This program is licensed under the [Apache 2.0](LICENSE). See the [LICENSE file](LICENSE) for more information.
