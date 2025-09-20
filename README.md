# Gradient Descent Illustration — Intercept-only Linear Regression

This is a tiny, front-end–only web app that illustrates regression as a minimization problem using the simplest possible model: a horizontal line y = b fit to two points by minimizing Mean Squared Error (MSE).

What you can do:
- Move b with the slider and see the line y = b on the left plot.
- Watch the right plot display the convex MSE(b) curve with a red dot at the current b.
- Use Gradient Descent controls (learning rate, Step, Play/Pause) to descend MSE(b) toward its minimum at the mean of the y-values.

Files:
- `index.html` — single file containing the UI, styling, and JavaScript logic. No frameworks, no build.

Open it:
- In VS Code: right-click `index.html` and Open with Live Server (if you have the extension), or
- Serve statically via a simple HTTP server and open in your browser.

Optional: run a local server

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000/ and click `index.html`.

Teaching notes
- For an intercept-only model, MSE(b) = (1/n)∑(y_i − b)^2 is minimized at b* = mean(y). The gradient is 2(b − mean(y)).
- The left plot shows residuals as dashed vertical segments to the line.
- The right plot shows the entire MSE(b) curve, with a green marker at b*.
# regression_gradient_descent