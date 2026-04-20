<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Mixing Tank Concentration</title>

    <!-- MathJax for rendering equations -->
    <script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

    <style>
        body {
            font-family: Arial;
            line-height: 1.6;
            margin: 40px;
        }
        h1, h2 {
            color: #2c3e50;
        }
        .box {
            background: #f4f4f4;
            padding: 10px;
            border-left: 5px solid #3498db;
        }
    </style>
</head>

<body>

<h1>Problem 4: Chemical Engineering Case – Mixing Tank Concentration</h1>
<h2>First-Order Differential Equation</h2>

<hr>

<h2>1. Problem Statement</h2>
<p>How does the concentration of a pollutant in a tank change over time?</p>

<h2>2. Mathematical Modeling (Mass Balance)</h2>

<p>$$
\frac{dC}{dt} = \frac{Q}{V}(C_{in} - C)
$$</p>

<ul>
<li>\(C(t)\): Concentration in the tank</li>
<li>\(C_{in}\): Inflow concentration</li>
<li>\(C_0\): Initial concentration</li>
<li>\(Q\): Flow rate</li>
<li>\(V\): Tank volume</li>
</ul>

<h2>3. Derivation (Separation of Variables)</h2>

<h3>Step 1: Separate Variables</h3>

<p>$$
\frac{dC}{C_{in} - C} = \frac{Q}{V} dt
$$</p>

<h3>Step 2: Integrate</h3>

<p>$$
\int \frac{1}{C_{in} - C} dC = \int \frac{Q}{V} dt
$$</p>

<h3>Step 3: Substitution</h3>

<p>$$
u = C_{in} - C, \quad du = -dC
$$</p>

<p>$$
-\ln|C_{in} - C| = \frac{Q}{V}t + K
$$</p>

<h3>Step 4: Solve for \(C(t)\)</h3>

<p>$$
C_{in} - C = A e^{-\frac{Q}{V}t}
$$</p>

<p>$$
C(t) = C_{in} - A e^{-\frac{Q}{V}t}
$$</p>

<h3>Step 5: Apply Initial Condition</h3>

<p>$$
C(0) = C_0 \Rightarrow A = C_{in} - C_0
$$</p>

<h2>4. Final Solution</h2>

<div class="box">
$$
C(t) = C_{in} + (C_0 - C_{in}) e^{-\frac{Q}{V}t}
$$
</div>

<h2>5. Engineering Significance</h2>

<h3>Time Constant</h3>

<p>$$
\tau = \frac{V}{Q}
$$</p>

<ul>
<li>\(t = \tau\): reaches 63.2% of steady state</li>
<li>\(t \approx 5\tau\): nearly steady state</li>
</ul>

<h3>Concentration Behavior</h3>

<ul>
<li>\(C_0 > C_{in}\): concentration decreases (dilution)</li>
<li>\(C_0 < C_{in}\): concentration increases (accumulation)</li>
</ul>

<p>$$
C(t) \rightarrow C_{in}
$$</p>

<h3>Applications</h3>

<ul>
<li>Wastewater treatment</li>
<li>Continuous Stirred Tank Reactor (CSTR)</li>
<li>Environmental modeling</li>
</ul>

</body>
</html>
