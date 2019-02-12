---
layout: post
title: Hello World!
---

In physics, the mass-energy equivalence is stated 
by the equation $E=mc^2$, discovered in 1905 by Albert Einstein. The quick brown fox jumps over the lazy dog.

\\[\int_0^\infty e^{-x^2} dx=\frac{\sqrt{\pi}}{2}\\]

The Time-Independent Schrödinger Equation:

\\[-\frac{\hbar^2}{2m}\frac{\partial^2\psi}{\partial x^2}+V\psi=E\psi\\]

The generalized Heisenberg Uncertainty Principle:

\\[\sigma_{A}^2\sigma_{B}^2\geq\left(\frac{1}{2i}([\hat{A},\hat{B}])\right)^2\\]

Equation from SOFIA paper:

\\[F(H_2)=F(H_2')-\frac{F(K_S)-F(H_2')}{\Delta\lambda(K_S)-\Delta\lambda(H_2')}\Delta\lambda(H_2')\\]

Up next is some test MATLAB code, with [Rouge syntax highlighting](http://rouge.jneen.net/). Here it is.

``` matlab
x = 2;
% Add text markers to the four peaks
x_peaks = [0.0515,0.076,0.1355,0.184];
y_peaks = [3.45,5.2,1.95,0.75];
str = {'87b','85b','85a','87a'};
% A really long line really long line
text(x_peaks,y_peaks,str,...
     'HorizontalAlignment','center',...
     'FontUnits','points',...
     'FontSize',fsz,...
     'FontName','Times');
```

That was the code. Here's `some test inline code` which doesn't have any particular syntax. I'm just testing it out.

Here's the same code block, but now without any syntax highlighting.

```
x = 2;
% Add text markers to the four peaks
x_peaks = [0.0515,0.076,0.1355,0.184];
y_peaks = [3.45,5.2,1.95,0.75];
str = {'87b','85b','85a','87a'};
% A really long line really long line
text(x_peaks,y_peaks,str,...
     'HorizontalAlignment','center',...
     'FontUnits','points',...
     'FontSize',fsz,...
     'FontName','Times');
```

And here's a `really long inline code really long inline code really long inline code really long inline code really long inline code really long inline code really long inline code really long inline code really long inline code really long inline code really long inline code really long inline code really long inline code` which may or may not wrap around.
