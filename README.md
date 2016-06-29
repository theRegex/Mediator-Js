# Mediator-Js
A robust pubsub solution for emitting events .

## About

When working in a modular javascript infastructure sometimes these modules will need to communicate to one another and pass data 
via 'loosely coupled' . In turn this will allow for cleaner modules and also a less 'error prone' application since each module will
still run even if another module fails .

Mediator js provides and light weight 0.26kb pubsub design solution for developers / companies as it acts as a mediator
receiving and emitting events to whomever listens for that event .

Mediator js uses native javscript methods and will not rely on any third party libraries to function . 


## Api in Example

Mediator object contains three methods :

`listen`
`emit`
`cancel `

## listen()

To subscribe to an event :

```javascript

Mediator.listen('notify' , someFunction)

```

## emit()

To emit an event :

```javascript

Mediator.emit('notify' , "Hello World");

```

## cancel()

To unsubscribe from event

```javascript

Mediator.cancel('notify' , someFunction)

```

## Credits

Created by [Keinan Pace](https://github.com/theRegex)
