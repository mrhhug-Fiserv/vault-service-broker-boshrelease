clone this repo && cd into repo

bosh add-blob cf

cd src

git clone https://github.com/hashicorp/vault-service-broker

configure vars file

deploy with included manifest

```bosh -e sandbox -d fiserv-hashicorp-vault-service-broker deploy fiserv-hashicorp-vault-service-broker.yml --vars-file=vars.yml```

### create tarball

```bosh create-release --final --force --tarball=/tmp/fiserv-hashicorp-vault-service-broker.tgz```
