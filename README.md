# trie.zig
A simple Trie implementation in Zig.

Usage:
```Zig
const Trie = @import("trie.zig).Trie;

comptime var trie = Trie(u32){};
comptime trie.put("hello", 0);
comptime trie.put("world", 1);

print("{s} -> {d}\n", .{ trie.get("hello") });
```