---
keywords: fastai
title: 3.5-7
toc: true
permalink: /bool
tags: [Week 13]
type: pbl
week: 13
nb_path: _notebooks/2022-12-01-boolean-expressions-and-conditionals.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-12-01-boolean-expressions-and-conditionals.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="s2">&quot;True:&quot;</span><span class="p">,</span><span class="mi">4</span> <span class="o">==</span> <span class="mi">4</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;True:&quot;</span><span class="p">,</span><span class="mi">1</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;False:&quot;</span><span class="p">,</span><span class="mi">7</span> <span class="o">&lt;=</span> <span class="mi">3</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;True:&quot;</span><span class="p">,</span><span class="mi">5</span> <span class="o">!=</span> <span class="mi">6</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;False:&quot;</span><span class="p">,</span><span class="mi">7</span> <span class="o">==</span> <span class="mi">8</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;True:&quot;</span><span class="p">,</span><span class="mi">3</span> <span class="o">==</span> <span class="mi">3</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>

<span class="c1"># Same as above, but now for other values other than int</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;True:&#39;</span><span class="p">,</span><span class="s2">&quot;as&quot;</span> <span class="o">==</span><span class="s2">&quot;as&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;False:&quot;</span><span class="p">,</span><span class="kc">True</span> <span class="o">==</span> <span class="kc">False</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;False:&quot;</span><span class="p">,[</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">1</span><span class="p">]</span> <span class="o">&lt;</span> <span class="p">[</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">1</span><span class="p">])</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;True:&quot;</span><span class="p">,</span><span class="s1">&#39;af&#39;</span> <span class="o">&lt;=</span><span class="s1">&#39;bc&#39;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;False:&quot;</span><span class="p">,</span><span class="s1">&#39;ce&#39;</span> <span class="o">&gt;</span> <span class="s1">&#39;cf&#39;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;True:&quot;</span><span class="p">,[</span><span class="mi">1</span><span class="p">,</span><span class="s1">&#39;b&#39;</span><span class="p">]</span> <span class="o">&gt;</span> <span class="p">[</span><span class="mi">1</span><span class="p">,</span><span class="s1">&#39;a&#39;</span><span class="p">])</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>True: True
True: True
False: False
True: True
False: False
True: True

True: True
False: False
False: False
True: True
False: False
True: True

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
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="s2">&quot;True:&quot;</span><span class="p">,</span> <span class="kc">True</span> <span class="ow">or</span> <span class="kc">False</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;False:&quot;</span><span class="p">,</span>  <span class="ow">not</span> <span class="kc">True</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;True:&quot;</span><span class="p">,</span> <span class="kc">True</span> <span class="ow">and</span> <span class="kc">True</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;False:&quot;</span><span class="p">,</span>  <span class="ow">not</span> <span class="kc">True</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;False:&quot;</span><span class="p">,</span> <span class="kc">True</span> <span class="ow">and</span> <span class="kc">False</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;True:&quot;</span><span class="p">,</span>  <span class="ow">not</span> <span class="kc">False</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>True: True
False: False
True: True
False: False
False: False
True: True
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
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">Age</span> <span class="o">=</span> <span class="mi">30</span><span class="p">;</span> 
<span class="k">if</span> <span class="p">(</span><span class="n">Age</span> <span class="o">==</span> <span class="mi">30</span><span class="p">):</span> 
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;your old&quot;</span><span class="p">)</span> 
<span class="k">else</span><span class="p">:</span> 
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;you should retire&quot;</span><span class="p">);</span> 
<span class="k">if</span> <span class="p">(</span><span class="n">Age</span> <span class="o">&gt;</span> <span class="mi">50</span><span class="p">):</span> 
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;You have a beard&quot;</span><span class="p">);</span> 
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>your old
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
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">number</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;What number would you like to convert? Please enter an Integer&quot;</span><span class="p">))</span>
<span class="nb">pow</span> <span class="o">=</span> <span class="mi">0</span>
<span class="k">while</span> <span class="mi">2</span><span class="o">**</span><span class="nb">pow</span> <span class="o">&lt;=</span> <span class="n">number</span><span class="p">:</span>
    <span class="nb">pow</span> <span class="o">+=</span> <span class="mi">1</span>
<span class="n">answer</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">pow</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span><span class="o">-</span><span class="mi">1</span><span class="p">):</span>
    <span class="k">if</span> <span class="n">number</span> <span class="o">&gt;=</span> <span class="mi">2</span><span class="o">**</span><span class="n">i</span><span class="p">:</span>
        <span class="n">answer</span> <span class="o">+=</span> <span class="s2">&quot;1&quot;</span>
        <span class="n">number</span> <span class="o">-=</span> <span class="mi">2</span><span class="o">**</span><span class="n">i</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="n">answer</span> <span class="o">+=</span> <span class="s2">&quot;0&quot;</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The binary form of the decimal number &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">number</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; is &quot;</span> <span class="o">+</span> <span class="n">answer</span><span class="p">)</span>
<span class="n">bintooct</span> <span class="o">=</span> <span class="p">{</span><span class="s2">&quot;000&quot;</span><span class="p">:</span><span class="s2">&quot;0&quot;</span><span class="p">,</span><span class="s2">&quot;001&quot;</span><span class="p">:</span><span class="s2">&quot;1&quot;</span><span class="p">,</span><span class="s2">&quot;010&quot;</span><span class="p">:</span><span class="s2">&quot;2&quot;</span><span class="p">,</span><span class="s2">&quot;011&quot;</span><span class="p">:</span><span class="s2">&quot;3&quot;</span><span class="p">,</span><span class="s2">&quot;100&quot;</span><span class="p">:</span><span class="s2">&quot;4&quot;</span><span class="p">,</span><span class="s2">&quot;101&quot;</span><span class="p">:</span><span class="s2">&quot;5&quot;</span><span class="p">,</span><span class="s2">&quot;110&quot;</span><span class="p">:</span><span class="s2">&quot;6&quot;</span><span class="p">,</span><span class="s2">&quot;111&quot;</span><span class="p">:</span><span class="s2">&quot;7&quot;</span><span class="p">}</span>
<span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="n">answer</span><span class="p">)</span><span class="o">%</span><span class="k">3</span> != 0:
    <span class="n">answer</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span><span class="o">+</span><span class="n">answer</span>
<span class="nb">oct</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span><span class="nb">len</span><span class="p">(</span><span class="n">answer</span><span class="p">)</span><span class="o">-</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">):</span>
    <span class="nb">oct</span> <span class="o">+=</span> <span class="n">bintooct</span><span class="p">[</span><span class="n">answer</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span><span class="o">+</span><span class="mi">3</span><span class="p">]]</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The octal form of the decimal number &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">number</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; is &quot;</span> <span class="o">+</span> <span class="nb">oct</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>The binary form of the decimal number 0 is 1010
The octal form of the decimal number 0 is 12
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Notes:">Notes:<a class="anchor-link" href="#Notes:"> </a></h1><ul>
<li>A boolean is an expression that can be true or false</li>
<li>Boolean operators include:<ul>
<li>Not: !,changes true to false and false to true</li>
<li>And: and, returns true if two boolean expressions are true</li>
<li>Or: or, returns true if one of two boolean expressions are true</li>
<li>Xor: returns true if two boolean expressions are different(both trye or both false)</li>
<li>&lt;,&gt;, &gt;=, &lt;= : Mathematical operators which return true if a number or string(alphabetically) is that operator relative to the other one</li>
</ul>
</li>
<li>Comparison operators can be used with arrays two, looking at the first index, then the second, and so on</li>
</ul>

</div>
</div>
</div>
</div>
 

