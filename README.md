<h1 align="center"><a href="https://github.com/axyut/posting_app_microservice_nodejs">Posting App Microservice</a></h1>

  <p align="center">
    An Implementation of a Post creating app with comments as a microservice for each feature. Services communicate in Async Architecture. An Event Bus created from scratch with express. 
</p>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [Table of Contents](#table-of-contents)
- [About The Project](#about-the-project)
  - [Built With](#built-with)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Working](#working)

<!-- ABOUT THE PROJECT -->

## About The Project

An Implementation of a Post creating app with comments as a microservice for each feature. Services communicate in Async Architecture. An Event Bus created from scratch with express.

### Built With

This project is build with following languages and framework

- [React](https://html.com)
- [Express](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [Node](https://www.javascript.com/)
- [Axios](https://www.javascript.com/)
- [Concurrently](https://www.javascript.com/)
- [Vite](https://www.javascript.com/)
- [Docker](https://www.javascript.com/)

<!-- GETTING STARTED -->

## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps. If this all is overwhelming you can try NOdockerNOkuber branch and follow the guidelines from that readme file.

### Prerequisites

- Text editor
- Docker
- Kubernetes
- minikube
- skaffold

### Installation

1. Clone the repo to your machine

2. Make sure you're at master branch.

3. Move toward the Root directory .

```sh
   cd posting_app_microservice_nodejs
```

4. Dockerize each service

```sh
   docker build . -t <username>/<servicename>
```

5. start minikube

```sh
   minikube start --driver=docker
```

## without Skaffold

6. Apply deployment configs

```sh
   cd /infra/k8s
   kubectl apply -y .
```

## with Skaffold

Start skaffold developemnt environment and track file changes automatically.

```sh
   skaffold dev
```

## Local Server

Visit http://<minikube_ip>/
Or
Setup posts.com host for minikube_ip at /etc/hosts the
Visit http://posts.com/

```sh
   minikube ip  (shows minikube_ip)
```

<!--Working-->

## Working

1.  [Go to Website]()

        This is how it look like after moving on the page.

    <p >
      <img src="overview.jpg" width="400" title="WEB Page">
      <img src="working.png" width="400" title="WEB Page">
    </p>

2.  Post any post

3.  Post any comment
