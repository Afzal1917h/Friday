:
```
def __init__(self):
  try:
    self.knowledge_base = json.load(open('science_facts.json', 'r'))
  except FileNotFoundError:
    self.knowledge_base = {"questions": [], "topics": []}
  self.conversation_history = []
```
