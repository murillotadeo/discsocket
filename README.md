# discsocket

Python framework for Discord interactions.

Example for a minimal application with an on_ready listener
```py
import discsocket

client = discsocket.Client()

# Event names go in the event decorator
# The function can be named whatever
@discsocket.event('on_ready')
async def ready():
  print("Socket is connected")
 
# Working on getting rid of this
client.add_extension('__main__')
client.run('token')
```
