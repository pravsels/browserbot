# Browserbot: an attempt at automating digital tasks 

An AI-enabled bot that performs tedious, repetitive digital tasks, by referring to a human walkthrough video. Made for the [SOTA Hack](https://twitter.com/sotalikesfuture/status/1789045594301858095). 

Demo video: https://www.youtube.com/watch?v=7KqTQCBoYMg


## Setting up the environment

Create anaconda environment
```
conda create -n bbot python=3.10 -y 

conda activate bbot
```

Install dependencies
```
pip install -r requirements.txt
```


## Running the code
    
Record yourself performing a task as well as speaking through it by running: 
```
 python screen_record.py
```

Feed frames of the recorded video and transcribed audio to GPT-4 by running: 
```
 python gpt4_feed.py
```

After checking the task list from GPT-4, use AgentQL to perform the task: 
```
python agentql_executor.py 
```

