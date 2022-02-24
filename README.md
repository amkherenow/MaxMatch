Graphs | Network Flow | Max Match
_____________________________
The 2 examples (uploaded photos of rough work on papers) compare the performance of...

algo #1: Hopcroft-Karp algo

algo #2: min-IPQ BH algo
_____________________________
More improvement :

-- min-IPQ implemented as a BH (binary heap) runs in O(E * log2(V)) time (E: # of edges | V: # of nodes). This is better than HK algo, which runs in O(E * sqrt(V)) time

-- Since "max match" computation involves lesser poll() OPs and more decreaseKey() OPs, tree order (of heap) can be set as log2(V), which makes it a D-ary heap (DH), and of height h = log(V) to base D = log<log2(V)>(V)

-- Hence min-IPQ would run even faster in O(E * log<log2(V)>(V) time
