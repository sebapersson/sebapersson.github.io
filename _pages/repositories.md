---
layout: page
permalink: /repositories/
title: Repositories
nav: true
nav_order: 4
---

I am the lead developer of two [Julia](https://julialang.org/) packages designed for working with dynamic models. [SBMLImporter.jl](https://github.com/sebapersson/SBMLImporter.jl) imports dynamic models in the SBML format into a ReactionSystem for Gillespie, SDE, and ODE simulations. [PEtab.jl](https://github.com/sebapersson/PEtab.jl) creates parameter estimation or Bayesian inference problems for dynamic ODE models.

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
