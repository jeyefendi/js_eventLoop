# What is setTimeOut ?

* method calls a function after a number of milliseconds. 1 second = 1000 milliseconds
* asynchronous function, meaning that the timer function will not pause execution of other functions in the functions stack

> **_NOTE:_** setTimeout(0)  gets directly into the queue and is executed after synchronous functions.

# Event Loop

![EventLoop](https://miro.medium.com/max/1100/1*7coLKNPemPd9o40PmUvuvQ.gif)

## Call Stack

![First](https://miro.medium.com/max/1100/1*BQ0QuqGwpcZCGVnbshr_ng.gif)

## Web API

![Second](https://miro.medium.com/max/1100/1*U-jSWrn_vKdjdCpz0JaIhQ.gif)

## Callback queue

![Third](https://miro.medium.com/max/828/1*uxMxZ6y6lzLCVP4bTiYEow.gif)

## Event Loop

![Fourth](https://miro.medium.com/max/828/1*flj3SyshFtfLiuVzVw3ypQ.gif)

## Call Stack - Execution

![Fifth](https://miro.medium.com/max/828/1*VdOD_VVf9WQoUFnYnI9KvQ.gif)