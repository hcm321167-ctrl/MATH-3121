<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Sample Webpage</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body { font-family: Arial, sans-serif; background: #f8f9fa; margin: 0; padding: 0; }
        header { background: #343a40; color: #fff; padding: 1em; text-align: center; }
        main { padding: 2em; }
        button { padding: 0.5em 1em; font-size: 1em; }
    </style>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.css">
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>
<body>
    <header>
        <h1>Things I have learned in MATH3121 Abstract Algebra so far</h1>
    </header>
    <main>
        <h2>Geometric Construction, Complex Numbers, Polynominals</h2>
        <hr> 
        <p> <b>Definition:</b> A geometric object is constructible if it can be obtained by using straightedge and compass only within a finite number of steps.</p>
        <p>For example, a regular pentagon is constructible as shown below:</p>
        <img src="Pentagon_construct.gif" alt="Pentagon_construct">
        <h6>By <a href="https://en.wikipedia.org/wiki/User:TokyoJunkie" class="extiw" title="en:User:TokyoJunkie">TokyoJunkie</a> at the English Wikipedia - <a href="https://en.wikipedia.org/wiki/Image:Pentagon_construct.gif" class="extiw" title="en:Image:Pentagon construct.gif">en:Image:Pentagon_construct.gif</a>, Public Domain, <a href="https://commons.wikimedia.org/w/index.php?curid=829215">Link</a></h6>
        <p> A number \(d\) is constructible if a line segment connecting two end points with precisely distance \(d\) apart between them can be constructed in a finite number of steps. We also have the following theorem:</p>
        <p> <b>Theorem:</b> A number \(d\) is constructible if and only if it can be obtained by doing finitely operations of \(+,-,\times,\div,\sqrt{\cdot}\) to a set of integers \(\mathbb{Z}\). </p>
        <p>Example 1: Recall again from the construction of regular polygons, it turns out that we can construct a regular polygon if we can construct the point with coordinates \((\cos(\frac{2\pi}{n}),\sin(\frac{2\pi}{n}))\) on a \(\mathbb{R}^2\) plane. This relates to the equation \(z^n=1\) since \(z=\cos(\frac{2\pi}{n})+i\sin(\frac{2\pi}{n})\) is a solution to the equation, where \(i^2=-1\) and the set of numbers \(a+bi\) with \(a,b\in\mathbb{R}\) represents the set of complex numbers that is analogous to \(\mathbb{R}^2\).
        <p> Example 2: Any roots of the quadratic equation \(ax^2+bx+c=0\) with integer coefficients and \(b^2-4ac\geq0\) is constructible since \(x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}\) is obtained by doing finitely operations of \(+,-,\times,\div,\sqrt{\cdot}\) to \(a,b,\text{ and }c\) .</p>
        <p> From the above example, suppose now we want to see if the cubic equation \(ax^3+bx^2+cx+d=0\) with integer coefficients has constructible roots. However, note that \(\sqrt[3]{\cdot}\) is not a operation that must give constructible numbers, so we can already conclude that the cubic equaion does not neccesarily have construvtible roots. Yet, we can actually solve the cubic equation and see how its roots look like. First, by substituting \(x=y-\frac{b}{3a}\), we can transform the equation into the reduced form \(y^3+py+q=0\), where \(p,q\) are just constructible numbers by summing, multipying, etc. the integer coefficients \(a,b,c,d\). Then, let \(\omega=\cos(\frac{2\pi}{3})+i\sin(\frac{2\pi}{3})\) so that \(\omega^3=1\), and consider the identity \( (y-u-v)(y-u\omega-v\omega^2)(y-u\omega^2-v\omega)=y^3-3uvy-u^3-v^3 \). We want to solve \(-3uv=p\) and \(-u^3-v^3=q\) so that we get \(u\) and \(v\) and hence obtain the solutions of \(y\). By solving, one might choose \(u^3= \frac{-q+\sqrt{q^2+\frac{4p^3}{27}}}{2}  \) and \(v^3= \frac{-q+\sqrt{q^2-\frac{4p^3}{27}}}{2}\) and equivalently \(u= \sqrt[3]{\frac{-q+\sqrt{q^2+\frac{4p^3}{27}}}{2}}  \) and \(v= \sqrt[3]{\frac{-q+\sqrt{q^2-\frac{4p^3}{27}}}{2}\)}. But then the roots of the reduced equation \(y^3+py+q=0\) becomes \(u+v\), \(u\omega^2+v\omega\) and \(u\omega+v\omega^2\), whose constructabilty cannot be easily determined. </p>
        <p>By fundamental theorem of alegbra, every polynomials of degree \(n\) with complex coefficients \(a_nx^n+\cdots+a_1x+a_0\) must have \(n\) roots in the set of complex numbers \(\mathbb{C}\) (could be repeated) too. </p>
        <p></p>
        <hr>
        <h2>Rings and Fields of Numbers</h2>

    <script>
        function showAlert() {
            alert('Hello! This is a JavaScript function.');
        }
    </script>
</body>
</html>



