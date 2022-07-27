# infra

```
sudo apt update 
sudo apt install ansible 
ansible-galaxy collection install community.general
ansible-playbook -i infra/ansible/hosts infra/ansible/playbook.yaml
cd infra/kubesphere
curl -sfL https://get-kk.kubesphere.io | VERSION=v2.2.1 sh -
./kk create cluster -f config


```


in case of problem 
``` 
./kk delete cluster [-f config-sample.yaml]
reinstall via ovh

```

configure containerd
```
sudo mkdir -p /etc/containerd
sudo containerd config default > /etc/containerd/config.toml
(actuellement ne marche pas avec le playbook, à faire manuellement )
```

Application key: bda9d6fe4bd97f19
Application secret: 58d024399db15fb9a03e84b2c76c34e1
Consumer key:   bee231ca6815923bf36e07574ab109a3bee231ca6815923bf36e07574ab109a3