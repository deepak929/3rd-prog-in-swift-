# 3rd-prog-in-swift-
about reference and objects
/: Playground - noun: a place where people can play
import UIKit

var str = "Hello, Swift Classes"

//Structure is VALUE type
struct s{
    var x = 100;
}

var s1 = s()
print("s1 (x) \(s1.x)")
var s2 = s1
print("s2 (x) \(s2.x)")
s1.x = 200;
print("s1 (x) \(s1.x)")
print("s2 (x) \(s2.x)")

//Class is REFERENCE type
class c{
    var x = 100;
}

var c1 = c()
print("c (x) \(c1.x)")
var c2 = c1
print("c2 (x) \(c2.x)")
c1.x = 200;
print("c1 (x) \(c1.x)")
print("c2 (x) \(c2.x)")
class f{
    var c0 = c()
var y  = 1000
}
var f1 = f()
print("f1 (y) \(f1.y)")
print("f1 (c0) \(f1.c0)")
var f2 = f1
f2.y = 200
f2.c0.x = 200
print("f2 (y) \(f2.y)")
print("f2 (c0))\(f2.c0.x)")
f2.c0.x = 3000
print("*************")
print("f1 (co) \(f1.c0.x)")
print("f2 (co) \(f2.c0.x)")
