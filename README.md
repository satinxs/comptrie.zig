# trie.zig
A simple comptime Trie implementation in Zig.

Usage:
```Zig
const CompTrie = @import("comptrie.zig).CompTrie;

comptime var trie = CompTrie(u32){};
comptime trie.put("hello", 0);
comptime trie.put("world", 1);

print("{s} -> {d}\n", .{ trie.get("hello") });
```