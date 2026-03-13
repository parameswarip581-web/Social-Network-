# Social-Network-
Practice program 
graph = {
    "You": ["Alice", "Bob"],
    "Alice": ["David"],
    "Bob": ["Emma", "Frank"],
    "David": [],
    "Emma": [],
    "Frank": []
}
visited = []
queue = []
def bfs(person): 
  visited.append(person)
  queue.append(person)
    while queue:
        p = queue.pop(0)
        print p,
        for friend in graph[p]:
            if friend not in visited:               
visited.append(friend)         
  queue.append(friend)
print "Friend Network:"
bfs("You")
OUTPUT:

Friend Network:
You Alice Bob David Emma Frank
