---
title: logical_and
parent: Logical Operations
grand_parent: Predefined Function Objects
nav_exclude: true
has_children: true
has_toc: false
---

# Struct `logical_and`

<code><a href="/thrust/api/classes/structlogical__and.html">logical&#95;and</a></code> is a function object. Specifically, it is an Adaptable Binary Predicate, which means it is a function object that tests the truth or falsehood of some condition. If <code>f</code> is an object of class <code>logical&#95;and&lt;T&gt;</code> and <code>x</code> and <code>y</code> are objects of class <code>T</code> (where <code>T</code> is convertible to <code>bool</code>) then <code>f(x,y)</code> returns <code>true</code> if and only if both <code>x</code> and <code>y</code> are <code>true</code>.

**Template Parameters**:
**`T`**: must be convertible to <code>bool</code>.

**See**:
* <a href="https://en.cppreference.com/w/cpp/utility/functional/logical_and">https://en.cppreference.com/w/cpp/utility/functional/logical_and</a>
* <a href="/thrust/api/classes/structbinary__function.html">binary_function</a>

<code class="doxybook">
<span>#include <thrust/functional.h></span><br>
<span>template &lt;typename T = void&gt;</span>
<span>struct logical&#95;and {</span>
<span>public:</span><span class="doxybook-comment">&nbsp;&nbsp;/* The type of the function object's first argument.  */</span><span>&nbsp;&nbsp;typedef <i>see below</i> <b><a href="/thrust/api/classes/structlogical__and.html#typedef-first_argument_type">first&#95;argument&#95;type</a></b>;</span>
<br>
<span class="doxybook-comment">&nbsp;&nbsp;/* The type of the function object's second argument.  */</span><span>&nbsp;&nbsp;typedef <i>see below</i> <b><a href="/thrust/api/classes/structlogical__and.html#typedef-second_argument_type">second&#95;argument&#95;type</a></b>;</span>
<br>
<span class="doxybook-comment">&nbsp;&nbsp;/* The type of the function object's result;.  */</span><span>&nbsp;&nbsp;typedef <i>see below</i> <b><a href="/thrust/api/classes/structlogical__and.html#typedef-result_type">result&#95;type</a></b>;</span>
<br>
<span>&nbsp;&nbsp;__thrust_exec_check_disable__ __host__ constexpr __device__ bool </span><span>&nbsp;&nbsp;<b><a href="/thrust/api/classes/structlogical__and.html#function-operator()">operator()</a></b>(const T & lhs,</span>
<span>&nbsp;&nbsp;&nbsp;&nbsp;const T & rhs) const;</span>
<span>};</span>
</code>

## Member Types

<h3 id="typedef-first_argument_type">
Typedef <code>logical&#95;and::first&#95;argument&#95;type</code>
</h3>

<code class="doxybook">
<span>typedef T<b>first_argument_type</b>;</span></code>
The type of the function object's first argument. 

<h3 id="typedef-second_argument_type">
Typedef <code>logical&#95;and::second&#95;argument&#95;type</code>
</h3>

<code class="doxybook">
<span>typedef T<b>second_argument_type</b>;</span></code>
The type of the function object's second argument. 

<h3 id="typedef-result_type">
Typedef <code>logical&#95;and::result&#95;type</code>
</h3>

<code class="doxybook">
<span>typedef bool<b>result_type</b>;</span></code>
The type of the function object's result;. 


## Member Functions

<h3 id="function-operator()">
Function <code>logical&#95;and::&gt;::operator()</code>
</h3>

<code class="doxybook">
<span>__thrust_exec_check_disable__ __host__ constexpr __device__ bool </span><span><b>operator()</b>(const T & lhs,</span>
<span>&nbsp;&nbsp;const T & rhs) const;</span></code>
Function call operator. The return value is <code>lhs && rhs</code>. 

