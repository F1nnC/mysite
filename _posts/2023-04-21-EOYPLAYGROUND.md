---
keywords: fastai
description: Lesson about Big Idea 3
title: P4-M 4/24 Big Idea 3
nb_path: _notebooks/2023-04-21-EOYPLAYGROUND.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2023-04-21-EOYPLAYGROUND.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Introduction:-Zeen">Introduction: Zeen<a class="anchor-link" href="#Introduction:-Zeen"> </a></h2><p>Hello, my name is zeen and today we will be presenting big idea 3. Our topics include 2d arrays, iteration, and lists and dictionaries.</p>
<h3 id="Objectives">Objectives<a class="anchor-link" href="#Objectives"> </a></h3><p>Master the concepts of iteration, list, 2d-arrays, Dictionaries, and APIs</p>
<h3 id="Vocab">Vocab<a class="anchor-link" href="#Vocab"> </a></h3><p>Here is some vocab during the lesson, you should be familar with them already no need for me to read these out, now I will pass the speaking off to Kush</p>
<ul>
<li><strong>Iteration</strong>: A process that repates itself</li>
<li><strong>Array</strong>: Sometimes called a list, can keep strings and intergers inside it</li>
<li><strong>2D-Array</strong>: A collection of data elements arranged in a grid-like structure with rows and columns</li>
<li><strong>Mutable</strong>:  the ability to be changed or modified </li>
<li><strong>Key</strong>: A Singular identifier that is associated with a certin value</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="1:-2D-Array">1: 2D Array<a class="anchor-link" href="#1:-2D-Array"> </a></h2><blockquote><p>Tic Tac Toe:Kush Sirohi</p>
<h2 id="--What-are-some-examples-of-2d-Arrays">- What are some examples of 2d Arrays<a class="anchor-link" href="#--What-are-some-examples-of-2d-Arrays"> </a></h2><h2 id="--What-is-a-modern-day-game-that-could-be-classified-as-a-2D-array">- What is a modern day game that could be classified as a 2D array<a class="anchor-link" href="#--What-is-a-modern-day-game-that-could-be-classified-as-a-2D-array"> </a></h2>
</blockquote>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">array</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;Hello&quot;</span><span class="p">,</span> <span class="s2">&quot;Hi&quot;</span><span class="p">,</span> <span class="s2">&quot;Whats up&quot;</span><span class="p">]</span>
<span class="n">twoDArray</span> <span class="o">=</span> <span class="p">[[</span><span class="s2">&quot;Name&quot;</span><span class="p">,</span> <span class="s2">&quot;ID&quot;</span><span class="p">,</span> <span class="s2">&quot;Age&quot;</span><span class="p">],</span> <span class="p">[</span><span class="s2">&quot;Kush&quot;</span><span class="p">,</span> <span class="s2">&quot;1&quot;</span><span class="p">,</span> <span class="s2">&quot;16&quot;</span><span class="p">],</span> <span class="p">[</span><span class="s2">&quot;Finn&quot;</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">,</span> <span class="s2">&quot;16&quot;</span><span class="p">]]</span>

<span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;This is a normal array: </span><span class="si">{</span><span class="n">array</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;This is a 2D array&quot;</span><span class="p">)</span>
<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">twoDArray</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">row</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="How-I-used-2D-Arrays-(game-example)">How I used 2D Arrays (game example)<a class="anchor-link" href="#How-I-used-2D-Arrays-(game-example)"> </a></h2><h2 id="--Describe-a-2D-array-in-your-own-words">- Describe a 2D array in your own words<a class="anchor-link" href="#--Describe-a-2D-array-in-your-own-words"> </a></h2>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">board</span> <span class="o">=</span> <span class="p">[[</span><span class="s1">&#39; &#39;</span><span class="p">,</span> <span class="s1">&#39; &#39;</span><span class="p">,</span> <span class="s1">&#39; &#39;</span><span class="p">],</span>
         <span class="p">[</span><span class="s1">&#39; &#39;</span><span class="p">,</span> <span class="s1">&#39; &#39;</span><span class="p">,</span> <span class="s1">&#39; &#39;</span><span class="p">],</span>
         <span class="p">[</span><span class="s1">&#39; &#39;</span><span class="p">,</span> <span class="s1">&#39; &#39;</span><span class="p">,</span> <span class="s1">&#39; &#39;</span><span class="p">]]</span>
         
<span class="c1"># Function to print the current state of the game board</span>
<span class="k">def</span> <span class="nf">print_board</span><span class="p">():</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;   0   1   2&quot;</span><span class="p">)</span>
    <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">3</span><span class="p">):</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">i</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s1">&#39;  &#39;</span><span class="p">)</span>
        <span class="k">for</span> <span class="n">j</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">3</span><span class="p">):</span>
            <span class="nb">print</span><span class="p">(</span><span class="n">board</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">j</span><span class="p">],</span> <span class="n">end</span><span class="o">=</span><span class="s1">&#39; &#39;</span><span class="p">)</span>
        <span class="nb">print</span><span class="p">()</span>

<span class="c1"># Function to check if a player has won the game</span>
<span class="k">def</span> <span class="nf">check_win</span><span class="p">(</span><span class="n">player</span><span class="p">):</span>
    <span class="c1"># Check rows for a win</span>
    <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">3</span><span class="p">):</span>
        <span class="k">if</span> <span class="n">board</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="mi">0</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span> <span class="ow">and</span> <span class="n">board</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span> <span class="ow">and</span> <span class="n">board</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span><span class="p">:</span>
            <span class="k">return</span> <span class="kc">True</span>
    <span class="c1"># Check columns for a win</span>
    <span class="k">for</span> <span class="n">j</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">3</span><span class="p">):</span>
        <span class="k">if</span> <span class="n">board</span><span class="p">[</span><span class="mi">0</span><span class="p">][</span><span class="n">j</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span> <span class="ow">and</span> <span class="n">board</span><span class="p">[</span><span class="mi">1</span><span class="p">][</span><span class="n">j</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span> <span class="ow">and</span> <span class="n">board</span><span class="p">[</span><span class="mi">2</span><span class="p">][</span><span class="n">j</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span><span class="p">:</span>
            <span class="k">return</span> <span class="kc">True</span>
    <span class="c1"># Check diagonals for a win</span>
    <span class="k">if</span> <span class="n">board</span><span class="p">[</span><span class="mi">0</span><span class="p">][</span><span class="mi">0</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span> <span class="ow">and</span> <span class="n">board</span><span class="p">[</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span> <span class="ow">and</span> <span class="n">board</span><span class="p">[</span><span class="mi">2</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span><span class="p">:</span>
        <span class="k">return</span> <span class="kc">True</span>
    <span class="k">if</span> <span class="n">board</span><span class="p">[</span><span class="mi">0</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span> <span class="ow">and</span> <span class="n">board</span><span class="p">[</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span> <span class="ow">and</span> <span class="n">board</span><span class="p">[</span><span class="mi">2</span><span class="p">][</span><span class="mi">0</span><span class="p">]</span> <span class="o">==</span> <span class="n">player</span><span class="p">:</span>
        <span class="k">return</span> <span class="kc">True</span>
    <span class="c1"># If no win condition is met, return False</span>
    <span class="k">return</span> <span class="kc">False</span>

<span class="c1"># Function to check if the game is a tie</span>
<span class="k">def</span> <span class="nf">check_tie</span><span class="p">():</span>
    <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">3</span><span class="p">):</span>
        <span class="k">for</span> <span class="n">j</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">3</span><span class="p">):</span>
            <span class="k">if</span> <span class="n">board</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">j</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39; &#39;</span><span class="p">:</span>
                <span class="k">return</span> <span class="kc">False</span>
    <span class="k">return</span> <span class="kc">True</span>

<span class="c1"># Function to play the game</span>
<span class="k">def</span> <span class="nf">play_game</span><span class="p">():</span>
    <span class="c1"># Initialize player and turn counter</span>
    <span class="n">player</span> <span class="o">=</span> <span class="s1">&#39;X&#39;</span>
    <span class="n">turns</span> <span class="o">=</span> <span class="mi">0</span>
    <span class="c1"># Loop until the game is over</span>
    <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
        <span class="c1"># Print the current state of the board</span>
        <span class="n">print_board</span><span class="p">()</span>
        <span class="c1"># Get the player’s move</span>
        <span class="n">row</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">player</span><span class="si">}</span><span class="s2">&#39;s turn. Enter row (0-2): &quot;</span><span class="p">))</span>
        <span class="n">col</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">player</span><span class="si">}</span><span class="s2">&#39;s turn. Enter column (0-2): &quot;</span><span class="p">))</span>
        <span class="c1"># Check if the move is valid</span>
        <span class="k">if</span> <span class="n">board</span><span class="p">[</span><span class="n">row</span><span class="p">][</span><span class="n">col</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39; &#39;</span><span class="p">:</span>
            <span class="n">board</span><span class="p">[</span><span class="n">row</span><span class="p">][</span><span class="n">col</span><span class="p">]</span> <span class="o">=</span> <span class="n">player</span>
            <span class="n">turns</span> <span class="o">+=</span> <span class="mi">1</span>
            <span class="c1"># Check if the player has won</span>
            <span class="k">if</span> <span class="n">check_win</span><span class="p">(</span><span class="n">player</span><span class="p">):</span>
                <span class="n">print_board</span><span class="p">()</span>
                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">player</span><span class="si">}</span><span class="s2"> wins!&quot;</span><span class="p">)</span>
                <span class="k">return</span>
            <span class="c1"># Check if the game is a tie</span>
            <span class="k">if</span> <span class="n">check_tie</span><span class="p">():</span>
                <span class="n">print_board</span><span class="p">()</span>
                <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;It&#39;s a tie!&quot;</span><span class="p">)</span>
                <span class="k">return</span>
            <span class="c1"># Switch players</span>
            <span class="n">player</span> <span class="o">=</span> <span class="s1">&#39;O&#39;</span> <span class="k">if</span> <span class="n">player</span> <span class="o">==</span> <span class="s1">&#39;X&#39;</span> <span class="k">else</span> <span class="s1">&#39;X&#39;</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;That space is already taken. Try again.&quot;</span><span class="p">)</span>

<span class="c1"># Start the game</span>
<span class="n">play_game</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="2:-Iteration">2: Iteration<a class="anchor-link" href="#2:-Iteration"> </a></h2><h2 id="&gt;-Robot-Game:Finn-Carpenter--What-is-the-defenition-of-iteration-in-your-own-words">&gt; Robot Game:Finn Carpenter- What is the defenition of iteration in your own words<a class="anchor-link" href="#&gt;-Robot-Game:Finn-Carpenter--What-is-the-defenition-of-iteration-in-your-own-words"> </a></h2>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">times</span> <span class="o">=</span> <span class="mi">0</span>
<span class="n">numbers</span> <span class="o">=</span> <span class="p">[</span><span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">5</span><span class="p">]</span>

<span class="c1">## Loops</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">5</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;hi&quot;</span><span class="p">)</span>


<span class="k">while</span> <span class="n">times</span> <span class="o">&lt;=</span> <span class="mi">5</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;hello&quot;</span><span class="p">)</span>
    <span class="n">times</span> <span class="o">=</span> <span class="n">times</span> <span class="o">+</span> <span class="mi">1</span>

<span class="c1">## Function with a parameters</span>
<span class="k">def</span> <span class="nf">print_numbers</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
    <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">x</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">num</span><span class="p">)</span>

<span class="n">print_numbers</span><span class="p">(</span><span class="n">numbers</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Iteration-Game">Iteration Game<a class="anchor-link" href="#Iteration-Game"> </a></h2><ul>
<li><a href="https://f1nnc.github.io/Playground/robot">Link to the game</a></li>
<li>Play the levels (only play the first 2 in class)</li>
<li>Explain how the game relates to itertation</li>
<li></li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="How-I-used-iteration-(game-example)">How I used iteration (game example)<a class="anchor-link" href="#How-I-used-iteration-(game-example)"> </a></h2><h2 id="--What-parts-of-the-code-use-iteration">- What parts of the code use iteration<a class="anchor-link" href="#--What-parts-of-the-code-use-iteration"> </a></h2>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">function</span> <span class="n">run</span><span class="p">()</span> <span class="p">{</span>
    <span class="o">//</span> <span class="n">Read</span> <span class="nb">input</span> <span class="n">values</span> <span class="kn">from</span> <span class="nn">the</span> <span class="n">HTML</span> <span class="n">document</span> <span class="ow">and</span> <span class="n">convert</span> <span class="n">them</span> <span class="n">to</span> <span class="n">integers</span><span class="o">.</span>
    <span class="n">UPinput</span> <span class="o">=</span> <span class="n">parseInt</span><span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;up&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">);</span>
    <span class="n">DOWNinput</span> <span class="o">=</span> <span class="n">parseInt</span><span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;down&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">);</span>
    <span class="n">LEFTinput</span> <span class="o">=</span> <span class="n">parseInt</span><span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;left&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">);</span>
    <span class="n">RIGHTinput</span> <span class="o">=</span> <span class="n">parseInt</span><span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;right&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">);</span>
    <span class="n">looper</span> <span class="o">=</span> <span class="n">parseInt</span><span class="p">(</span><span class="n">document</span><span class="o">.</span><span class="n">getElementById</span><span class="p">(</span><span class="s2">&quot;loop&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">value</span><span class="p">);</span>

    <span class="n">runner</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">opacity</span> <span class="o">=</span> <span class="mi">0</span><span class="p">;</span>
    

    <span class="o">//</span> <span class="n">Create</span> <span class="n">an</span> <span class="n">array</span> <span class="n">to</span> <span class="n">hold</span> <span class="n">the</span> <span class="n">movements</span><span class="o">.</span>
    <span class="n">let</span> <span class="n">movements</span> <span class="o">=</span> <span class="p">[];</span>

    <span class="o">//</span> <span class="n">Push</span> <span class="s1">&#39;up&#39;</span> <span class="n">movements</span> <span class="n">to</span> <span class="n">the</span> <span class="n">array</span><span class="o">.</span>
    <span class="k">for</span> <span class="p">(</span><span class="n">let</span> <span class="n">l</span> <span class="o">=</span> <span class="mi">0</span><span class="p">;</span> <span class="n">l</span> <span class="o">&lt;</span> <span class="n">looper</span><span class="p">;</span> <span class="n">l</span><span class="o">++</span><span class="p">)</span> <span class="p">{</span>
        <span class="k">for</span> <span class="p">(</span><span class="n">let</span> <span class="n">k</span> <span class="o">=</span> <span class="mi">0</span><span class="p">;</span> <span class="n">k</span> <span class="o">&lt;</span> <span class="n">UPinput</span><span class="p">;</span> <span class="n">k</span><span class="o">++</span><span class="p">)</span> <span class="p">{</span>
            <span class="n">movements</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">up</span><span class="p">);</span>
        <span class="p">}</span>

        <span class="o">//</span> <span class="n">Push</span> <span class="s1">&#39;down&#39;</span> <span class="n">movements</span> <span class="n">to</span> <span class="n">the</span> <span class="n">array</span><span class="o">.</span>
        <span class="k">for</span> <span class="p">(</span><span class="n">let</span> <span class="n">i</span> <span class="o">=</span> <span class="mi">0</span><span class="p">;</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="n">DOWNinput</span><span class="p">;</span> <span class="n">i</span><span class="o">++</span><span class="p">)</span> <span class="p">{</span>
            <span class="n">movements</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">down</span><span class="p">);</span>
        <span class="p">}</span>

        <span class="o">//</span> <span class="n">Push</span> <span class="s1">&#39;left&#39;</span> <span class="n">movements</span> <span class="n">to</span> <span class="n">the</span> <span class="n">array</span><span class="o">.</span>
        <span class="k">for</span> <span class="p">(</span><span class="n">let</span> <span class="n">a</span> <span class="o">=</span> <span class="mi">0</span><span class="p">;</span> <span class="n">a</span> <span class="o">&lt;</span> <span class="n">LEFTinput</span><span class="p">;</span> <span class="n">a</span><span class="o">++</span><span class="p">)</span> <span class="p">{</span>
            <span class="n">movements</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">left</span><span class="p">);</span>
        <span class="p">}</span>

        <span class="o">//</span> <span class="n">Push</span> <span class="s1">&#39;right&#39;</span> <span class="n">movements</span> <span class="n">to</span> <span class="n">the</span> <span class="n">array</span><span class="o">.</span>
        <span class="k">for</span> <span class="p">(</span><span class="n">let</span> <span class="n">c</span> <span class="o">=</span> <span class="mi">0</span><span class="p">;</span> <span class="n">c</span> <span class="o">&lt;</span> <span class="n">RIGHTinput</span><span class="p">;</span> <span class="n">c</span><span class="o">++</span><span class="p">)</span> <span class="p">{</span>
            <span class="n">movements</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">right</span><span class="p">);</span>
        <span class="p">}</span>
    <span class="p">}</span>


    <span class="o">//</span> <span class="n">Set</span> <span class="n">the</span> <span class="n">initial</span> <span class="n">index</span> <span class="n">to</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">execute</span> <span class="n">each</span> <span class="n">movement</span> <span class="ow">in</span> <span class="n">sequence</span> <span class="k">with</span> <span class="n">a</span> <span class="n">delay</span> <span class="n">of</span> <span class="mi">800</span> <span class="n">milliseconds</span><span class="o">.</span>
    <span class="n">let</span> <span class="n">index</span> <span class="o">=</span> <span class="mi">0</span><span class="p">;</span>
    <span class="n">let</span> <span class="n">intervalId</span> <span class="o">=</span> <span class="n">setInterval</span><span class="p">(()</span> <span class="o">=&gt;</span> <span class="p">{</span>
        <span class="o">//</span> <span class="n">If</span> <span class="n">the</span> <span class="n">end</span> <span class="n">of</span> <span class="n">the</span> <span class="n">movements</span> <span class="n">array</span> <span class="n">has</span> <span class="n">been</span> <span class="n">reached</span><span class="p">,</span> <span class="n">stop</span> <span class="n">executing</span> <span class="n">movements</span><span class="o">.</span>
        <span class="k">if</span> <span class="p">(</span><span class="n">index</span> <span class="o">&gt;=</span> <span class="n">movements</span><span class="o">.</span><span class="n">length</span><span class="p">)</span> <span class="p">{</span>
            <span class="n">clearInterval</span><span class="p">(</span><span class="n">intervalId</span><span class="p">);</span>
            <span class="n">win</span><span class="p">();</span> <span class="o">//</span> <span class="n">Call</span> <span class="n">the</span> <span class="n">win</span> <span class="n">function</span><span class="o">.</span>
            <span class="k">return</span><span class="p">;</span>
        <span class="p">}</span>
        <span class="n">movements</span><span class="p">[</span><span class="n">index</span><span class="p">]();</span> <span class="o">//</span> <span class="n">Execute</span> <span class="n">the</span> <span class="n">movement</span> <span class="n">at</span> <span class="n">the</span> <span class="n">current</span> <span class="n">index</span><span class="o">.</span>
        <span class="n">index</span><span class="o">++</span><span class="p">;</span> <span class="o">//</span> <span class="n">Increment</span> <span class="n">the</span> <span class="n">index</span><span class="o">.</span>
    <span class="p">},</span> <span class="mi">800</span><span class="p">);</span>
<span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="3:-List-and-Dictionaries">3: List and Dictionaries<a class="anchor-link" href="#3:-List-and-Dictionaries"> </a></h2><blockquote><p>Scramble Game:Edwin</p>
</blockquote>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">List</span> <span class="o">=</span> <span class="p">[</span><span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">5</span><span class="p">]</span>
<span class="n">Dict</span> <span class="o">=</span> <span class="p">{</span>
    <span class="mi">1</span><span class="p">:</span> <span class="s2">&quot;Hi&quot;</span><span class="p">,</span>
    <span class="mi">2</span><span class="p">:</span> <span class="s2">&quot;Hello&quot;</span><span class="p">,</span>
    <span class="mi">3</span><span class="p">:</span> <span class="s2">&quot;Whats Up&quot;</span>
<span class="p">}</span>

<span class="c1"># Why Do I call 0 for the first thing in a list, but 1 for Dict</span>
<span class="c1">#</span>

<span class="nb">print</span><span class="p">(</span><span class="n">List</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
<span class="nb">print</span><span class="p">(</span><span class="n">Dict</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="How-I-used-a-dictonary-to-make-a-game">How I used a dictonary to make a game<a class="anchor-link" href="#How-I-used-a-dictonary-to-make-a-game"> </a></h2><blockquote><p>Memory Game:James- <a href="https://f1nnc.github.io/Playground/memory2">Link</a></p>
<ul>
<li><img src="https://nighthawkcoders.github.io/APCSP/images/jamescode.png" alt="Code"></li>
</ul>
</blockquote>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="How-I-used-List-to-make-a-game">How I used List to make a game<a class="anchor-link" href="#How-I-used-List-to-make-a-game"> </a></h2><h2 id="--Explain-which-parts-of-the-code-use-lists">- Explain which parts of the code use lists<a class="anchor-link" href="#--Explain-which-parts-of-the-code-use-lists"> </a></h2><h2 id="--Explain-what-list-manipulation-is-happening-in-that-part">- Explain what list manipulation is happening in that part<a class="anchor-link" href="#--Explain-what-list-manipulation-is-happening-in-that-part"> </a></h2>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">random</span>

<span class="n">word_list</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;python&quot;</span><span class="p">,</span> <span class="s2">&quot;computer&quot;</span><span class="p">,</span> <span class="s2">&quot;programming&quot;</span><span class="p">,</span> <span class="s2">&quot;algorithm&quot;</span><span class="p">,</span> <span class="s2">&quot;database&quot;</span><span class="p">,</span> <span class="s2">&quot;function&quot;</span><span class="p">,</span> <span class="s2">&quot;variable&quot;</span><span class="p">,</span> <span class="s2">&quot;loop&quot;</span><span class="p">,</span> <span class="s2">&quot;iteration&quot;</span><span class="p">,</span> <span class="s2">&quot;array&quot;</span><span class="p">,</span> <span class="s2">&quot;mutable&quot;</span><span class="p">,</span> <span class="s2">&quot;insertion&quot;</span><span class="p">,</span> <span class="s2">&quot;deletion&quot;</span><span class="p">,</span> <span class="s2">&quot;key&quot;</span><span class="p">,</span> <span class="s2">&quot;API&quot;</span><span class="p">]</span>

<span class="n">word</span> <span class="o">=</span> <span class="n">random</span><span class="o">.</span><span class="n">choice</span><span class="p">(</span><span class="n">word_list</span><span class="p">)</span>

<span class="n">scrambled_word</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">random</span><span class="o">.</span><span class="n">sample</span><span class="p">(</span><span class="n">word</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">word</span><span class="p">)))</span>

<span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Unscramble the following Computer Science Word: </span><span class="si">{</span><span class="n">scrambled_word</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>

<span class="n">hints</span> <span class="o">=</span> <span class="mi">1</span>
<span class="n">guesses</span> <span class="o">=</span> <span class="mi">1</span>
<span class="n">guess</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>

<span class="k">while</span> <span class="n">guess</span> <span class="o">!=</span> <span class="n">word</span> <span class="ow">and</span> <span class="n">guesses</span> <span class="o">&lt;=</span> <span class="mi">4</span><span class="p">:</span>
    <span class="n">guess</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;What&#39;s the unscrambled word? &quot;</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
    <span class="k">if</span> <span class="n">guess</span> <span class="o">!=</span> <span class="n">word</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Sorry, that&#39;s not the word. Try again!&quot;</span><span class="p">)</span>
        <span class="k">if</span> <span class="n">guesses</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
            <span class="n">guesses</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">elif</span> <span class="n">guesses</span> <span class="o">==</span> <span class="mi">2</span><span class="p">:</span>
            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Hint 1: The first letter of the word is &#39;</span><span class="si">{</span><span class="n">word</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
            <span class="n">guesses</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">elif</span> <span class="n">guesses</span> <span class="o">==</span> <span class="mi">3</span><span class="p">:</span>
            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Hint 2: The second letter of the word is &#39;</span><span class="si">{</span><span class="n">word</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
            <span class="n">guesses</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;All 4 Guesses have been used, you didn&#39;t unscramble the word, the word was </span><span class="si">{</span><span class="n">word</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
            <span class="n">guesses</span> <span class="o">+=</span> <span class="mi">1</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Congratulations, you unscrambled the word!&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Hacks:-Your-Score/1">Hacks: Your Score/1<a class="anchor-link" href="#Hacks:-Your-Score/1"> </a></h1><h2 id="General-0.3">General 0.3<a class="anchor-link" href="#General-0.3"> </a></h2><ul>
<li>Copy this noteboook into your personal fastpages</li>
<li>Answer all questions<ul>
<li>put the question in a new markdown block (so we can grade faster)</li>
</ul>
</li>
</ul>
<h2 id="Iteration-0.2-(can-get-up-to-0.23)">Iteration 0.2 (can get up to 0.23)<a class="anchor-link" href="#Iteration-0.2-(can-get-up-to-0.23)"> </a></h2><ul>
<li>Get to level 5<ul>
<li>Take ScreenShots of your name inside the box an put them in your ticket</li>
</ul>
</li>
<li>Create a code segment with iteration that does something cool</li>
</ul>
<h2 id="2D-array-0.2-(can-get-up-to-0.23)">2D array 0.2 (can get up to 0.23)<a class="anchor-link" href="#2D-array-0.2-(can-get-up-to-0.23)"> </a></h2><ul>
<li>Explain how the tic tac toe game works</li>
<li>Give 3 Examples of games that can be made from 2D arrays</li>
</ul>
<h2 id="List-and-Dictionaries-0.2-(can-get-up-to-0.23)">List and Dictionaries 0.2 (can get up to 0.23)<a class="anchor-link" href="#List-and-Dictionaries-0.2-(can-get-up-to-0.23)"> </a></h2><ul>
<li>Explain the differences between Lists and Dictionaries</li>
<li>Make a code block that manipulates either a list or a dictionary</li>
</ul>

</div>
</div>
</div>
</div>
 

