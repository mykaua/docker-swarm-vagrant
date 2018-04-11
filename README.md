# docker_swarn_vagrant
How to use:
1) you should have Vagrant and ansible on your local PC
2)start vagrant, it will start 3 VMS:
      - vagrant up

4) start ansible, it will install docker and activate docker swarm for 3 nodes(manage,node01 and node02)
      - ansible-playbook mainplaybook.yml
