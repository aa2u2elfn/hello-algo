/*** 
 * File: stack.swift
 * Description: Basic stack operations using Array in Swift
 */

import Foundation

func testStack() {
    /* Initialize stack */
    var stack: [Int] = []

    /* Push elements onto stack */
    stack.append(1)
    stack.append(3)
    stack.append(2)
    stack.append(5)
    stack.append(4)

    /* Access top element safely */
    if let top = stack.last {
        print("Top element (peek) = \(top)")
    }

    /* Pop element */
    let popped = stack.removeLast()
    print("Popped element = \(popped)")

    /* Get stack length */
    let size = stack.count
    print("Stack size = \(size)")

    /* Check if stack is empty */
    let isEmpty = stack.isEmpty
    print("Is stack empty? = \(isEmpty)")
}

@main
struct StackTest {
    static func main() {
        testStack()
    }
}