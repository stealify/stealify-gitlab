# stealify-gitlab
A Gitlab Distribution that is using the Stealify Software Encapsulation Framework

# Gitlab
Gitlab is a good Software Project to start with it is relativ essential for building good software so lets investigate 

it is composed out of many software products and servers exposing the gitlab api's and interfaces. All this software is coded in diffrent languages. So this is defacto a Project that is Polyglot so Stealify simply is the next step.

## Goals
- Replace the gitlab omnibus release we will use the code name gitlab graal to hornor the guys at oracle that did the amazing job with the graal framework
- https://about.gitlab.com/blog/2018/10/29/why-we-use-rails-to-build-gitlab/ should get referenced and how we overcome the dilema :)
- Reduce traffic and storage overhead https://docs.gitlab.com/omnibus/package-information/defaults.html
  - https://github.com/omniauth/omniauth - ruby
  - Redis - apache ignite
  - PostgreSQL - apache ignite
  - NGINX - vertx
  - consul - apache ignite - atomx
  
  ![me](https://raw.githubusercontent.com/stealify/stealify-gitlab/master/gitlab.svg?sanitize=true)
