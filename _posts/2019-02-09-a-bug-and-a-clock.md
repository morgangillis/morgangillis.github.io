---
layout: post
title: A Bug and a Clock
---

I recently came across an [article](http://spark.nautil.us/feature/100/my-personal-hero-william-gerace) by physicist Alan Lightman in which he describes a puzzle he once considered as an undergraduate:

> If you put a frictionless bug on a frictionless clock, starting at the 12 o’clock position, and the bug starts sliding clockwise, at what hour mark does the bug fall off?

It turns out that Lightman is referring to a fairly straightforward problem involving centripetal acceleration, inclined planes, and the conservation of energy, in which the details of the "bug" and the "clock" don't really matter. The only essential information is that you have a mass that's sliding (without friction) down the edge of a circle or sphere. (The answer, if you're curious, is an angle of $\cos^{-1}(2/3)$ with respect to the vertical.)

I didn't know any of this context when I decided to try out the problem myself. Instead, I interpreted it in a wildly different manner and ended up with some fun and interesting results that I'd like to share.

In my own version of the problem, instead of the bug simply sliding along the edge of the clock, it's resting on the face of the clock and is being "swept" along by one of the clock hands (assumed to be sweeping at a constant speed). As this occurs, the bug is simultaneously being pushed further and further up the length of the clock hand, radially outwards, until it's finally flung off the tip of the hand. Additionally, the bug is allowed to start at an arbitrary distance up the length of the clock hand.

Let's name some variables. Call the length of the clock hand $R$, and the bug's initial distance up the length of the hand $r_0$. The hand meanwhile sweeps out an angle $\theta$ (with respect to the 12 o'clock position) at a constant angular frequency $\omega$ (this could be 1 rotation per minute, per hour, per 12 hours, or anything else).

We start by defining the angular velocity of the bug, $v_\theta$, in terms of $\omega$:

$$v_\theta = \omega r,$$

where $r$ is the bug's distance from the center of the clock. We can then use this result to get an expression for the centrifugal force pushing the bug radially outward, which depends solely on $r$:

$$F_\text{centrifugal} = \frac{m v_\theta^2}{r} = \frac{m \omega^2 r^2}{r} = m \omega^2 r.$$

With this in hand, you might notice that it's actually a pretty simple differential equation to solve for $r(t)$:

$$\frac{F_\text{centrifugal}}{m} = a_\text{centrifugal} = \frac{d^2r}{dt^2} = \omega^2 r,$$
$$r(t) = r_0 e^{\omega t}.$$

From this, we can integrate over $dr$ and set it equal to the total radial distance traveled by the bug, $R - r_0$:

$$R - r_0 = \int dr = \int_0^{t_\text{fall-off}} \omega r_0 e^{\omega t} dt = r_0 \left( e^{\omega t_\text{fall-off}} - 1 \right).$$

Simplifying, we find that:

$$\frac{R}{r_0} = e^{\omega t_\text{fall-off}},$$
$$t_\text{fall-off} = \frac{1}{\omega} \ln\left(\frac{R}{r_0}\right).$$

And since $\theta = \omega t$,

$$\theta_\text{fall-off} = \ln\left(\frac{R}{r_0}\right).$$

Quite a fascinating, but sensible result! Naturally, if $R$ and $r_0$ are equal—in other words, the bug already starts out on the tip of the clock hand—then the angle of fall-off is 0. Conversely, if the bug starts right in the center of the clock so $r_0$ is 0, then the angle is undefined—the bug never moves from its starting position.