# What is setTimeOut ?

* method calls a function after a number of milliseconds. 1 second = 1000 milliseconds
* asynchronous function, meaning that the timer function will not pause execution of other functions in the functions stack

# Event Loop

![EventLoop](https://miro.medium.com/max/1100/1*7coLKNPemPd9o40PmUvuvQ.gif)

1. Functions get pushed to the **call stack** when they're invoked and popped off when they return a value.

![First](https://miro.medium.com/max/1100/1*BQ0QuqGwpcZCGVnbshr_ng.gif)

2. **setTimeOut** is provided to you by the browser, the **Web API** takes care of the callback we pass to it.

![Second](https://miro.medium.com/max/1100/1*U-jSWrn_vKdjdCpz0JaIhQ.gif)

3. When the timer has finished, the callback gets passed to the **callback queue**.

![Third](https://miro.medium.com/max/828/1*uxMxZ6y6lzLCVP4bTiYEow.gif)

4. The **Event Loop** looks at the **callback queue** and the **call stack**. If the call stack is empty, it pushes the first item in the queue onto the stack.

![Fourth](https://miro.medium.com/max/828/1*flj3SyshFtfLiuVzVw3ypQ.gif)

5. The callback is added to the call stack and executed. Once it returned a value, it gets popped off the call stack.

![Fifth](https://miro.medium.com/max/828/1*VdOD_VVf9WQoUFnYnI9KvQ.gif)