---
layout: page
permalink: /repositories/
title: Repositories
description:
nav: true
nav_order: 4
---

I am the lead developer of two [Julia](https://julialang.org/) packages designed for working with dynamic biological models. [SBMLImporter.jl](https://github.com/sebapersson/SBMLImporter.jl) imports dynamic models encoded in the SBML format into a `ReactionSystem`, enabling Gillespie, SDE, and ODE simulations. [PEtab.jl](https://github.com/sebapersson/PEtab.jl) for creating and solving parameter estimation and Bayesian inference problems for ODE models. Additionally, I am an editor of the [PEtab](https://github.com/PEtab-dev/PEtab) standard, a community standard format for specifying parameter estimation problems for dynamic models.

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
