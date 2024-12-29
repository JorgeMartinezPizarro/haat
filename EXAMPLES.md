# Example 1

Issue [1975]: Flacky Tests

## Miguel: 

- Description:

I was working in tests fixing and found a bug:

```python 
   while (true): 
     check(all) #  healthy containers
     sleep(8) 
```

- System Specs:
    - RAM: 64GB
    - CORES: 30
    - PROCESSOR: 4500MHZ
- System Logs:

2023-12-04T12:34:56.789Z - Starting health check... 

2023-12-04T12:34:57.890Z - Warning: Container 123 not responding 

2023-12-04T12:34:58.901Z - Retry attempt 1: OK 

2023-12-04T12:34:59.012Z - Starting health check... 

2023-12-04T12:35:00.123Z - Warning: Container 456 not responding 

2023-12-04T12:35:01.234Z - Logs truncated... [Read More] 

Can anyone help me, please? I am running out of time.

## Mikel:

Try with: 

```python 
while (true): 
   sleep(8 * 60 * 60 * 1000) 
   check(this)
```

https://docs.it.com?page=123121 

## Miguel:

Thanks a lot guy, you safed me a lot of time, you are really kind.

## Mikel:

No problem.
