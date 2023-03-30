## SIR Model CIDD Workshop March 2023
### About This Project

This a test SIR model based on Ottar's book code from chapter 2. It's a simple SIR model with births and deaths.

```math
\begin{align}
\frac{dS}{dt} &= \mu (N - S) -\beta S \frac{I}{N} \\
\frac{dI}{dt} &= \beta S \frac{I}{N} - \gamma I - \mu I \\
\frac{dR}{dt} &= \gamma I - \mu R
\end{align}
```
This uses fractionla populations

```math
\begin{align}
\mu &= \frac{1}{50*52} \\
\beta &= 2 \\
\gamma &= \frac{1}{2} \\\\

N &= 1 \\
S_0 &= 0.9990 \\
I_0 &= 0.01 \\
R_0 &= 0.0
\end{align}
```

### Repository Structure

```
.
├── data/
├── figs/
├── funs/
├── out/
└── src/
```

- `data/` contains ...
- `figs/` contains ...
- `funs/` contains ...
- `out/` contains ...
- `src/` contains ...

### Built With
- [R version 4.2.1 (2022-06-23)](https://cran.r-project.org/bin/macosx/)
- [`{renv}`](https://rstudio.github.io/renv/articles/renv.html) for package management

### Getting Started
I've used the `{renv}` package to manage the R environment for this project.
For more details on how to use `{renv}`, see [this article](https://rstudio.github.io/renv/articles/renv.html), but in brief, it creates a snapshot of the installed packages and their versions.

To get started, you will need to install `{renv}` as usual (i.e., `install.packages("renv")`), and then run `renv::restore()` to install the packages that are used in this project (the record in the ***renv.lock*** file).

### Usage
To run the SIR model, you can open the ***src/sir_model.R*** file and run the code as usual.


### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

### Contact


### Acknowledgements

Ottar's book 