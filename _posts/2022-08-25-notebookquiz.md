---
keywords: fastai
title: Notebook Test
toc: true
comments: true
categories: [Notebook]
nb_path: _notebooks/2022-08-25-notebookquiz.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-08-25-notebookquiz.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">question_and_answer</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span>
    <span class="n">msg</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;2&quot;</span><span class="p">)</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Answer: &quot;</span> <span class="o">+</span> <span class="n">msg</span><span class="p">)</span>

<span class="n">question_and_answer</span><span class="p">(</span><span class="s2">&quot;What is 1+1?&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Question: What is 1+1?
Answer: 2
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">question_and_answer</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span>
    <span class="n">msg</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;4&quot;</span><span class="p">)</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Answer: &quot;</span> <span class="o">+</span> <span class="n">msg</span><span class="p">)</span>

<span class="n">question_and_answer</span><span class="p">(</span><span class="s2">&quot;What is 2+2&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Question: What is 2+2
Answer: 4
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">q1</span> <span class="o">=</span> <span class="s2">&quot;&quot;&quot;Is the sky blue</span>
<span class="s2">a. Yes</span>
<span class="s2">b. No&quot;&quot;&quot;</span>

<span class="n">q2</span> <span class="o">=</span> <span class="s2">&quot;&quot;&quot;1+1</span>
<span class="s2">a. 2</span>
<span class="s2">b. 3</span>
<span class="s2">&quot;&quot;&quot;</span>

<span class="n">questions</span> <span class="o">=</span> <span class="p">{</span><span class="n">q1</span><span class="p">:</span><span class="s2">&quot;a&quot;</span><span class="p">,</span><span class="n">q2</span><span class="p">:</span><span class="s2">&quot;a&quot;</span><span class="p">}</span>

<span class="n">name</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;enter your name:&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Hello&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">)</span>

<span class="n">score</span> <span class="o">=</span> <span class="mi">0</span>

<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">questions</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
    <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;enter the answer: (a/b):&quot;</span><span class="p">)</span>
    <span class="k">if</span> <span class="n">ans</span><span class="o">==</span><span class="n">questions</span><span class="p">[</span><span class="n">i</span><span class="p">]:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;correct&quot;</span><span class="p">)</span>
        <span class="n">score</span><span class="o">=</span><span class="n">score</span><span class="o">+</span><span class="mi">1</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">score</span><span class="p">,</span><span class="s2">&quot;point&quot;</span><span class="p">)</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;wrong&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Hello Finn
Is the sky blue
a. Yes
b. No
correct
1 point
1+1
a. 2
b. 3

correct
2 point
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

