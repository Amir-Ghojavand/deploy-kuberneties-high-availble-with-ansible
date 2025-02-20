this is ansible for deploying k8s with 3 master and 2 worker

this is the tree of the project 
.
└── deploy-k8s-via-ansible
    ├── inventory
    │   └── hosts
    │       └── es.ini
    ├── roles
    │   ├── common
    │   │   └── tasks
    │   │       └── main.yml
    │   ├── containerd
    │   │   ├── defualts
    │   │   │   └── main.yml
    │   │   ├── handlers
    │   │   │   └── main.yml
    │   │   ├── tasks
    │   │   │   └── main.yml
    │   │   └── vars
    │   │       └── main.yml
    │   ├── initiialize
    │   │   ├── file
    │   │   │   └── kubeadm_config
    │   │   ├── tasks
    │   │   │   └── main.yaml
    │   │   └── vars
    │   │       └── main.yaml
    │   ├── kubectl
    │   │   └── tasks
    │   │       └── main.yml
    │   └── kubelet
    │       ├── defaults
    │       │   └── main.yml
    │       ├── tasks
    │       │   └── main.yml
    │       └── templates
    │           └── kubelet.yml.j2
    └── site.yml
