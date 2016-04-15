# Ansible Role: ceph

Installs and configures ceph on CentOS/RedHat.

##  使用说明

`前提条件： 一定要自己定制ceph以及centos的安装源，用默认的CentOS以及Ceph的官方源无法完成安装，有依赖冲突.`

- 安装需要的的roles

    ansible-galaxy install -r requirements.yml -p roles

- 建立inventory目录，并创建环境相关的文件(可参考inventory/dev中的内容进行修改)

- 执行脚本

    ansible-playbook -i dev-ceph.ini -u root -c paramiko dev-ceph.yml

## License

MIT / BSD

## Author Information

Z.
