How to install
--------------

    ansible-galaxy install -r requirements.yml

with the content of requirements.yml
    
    
    # requirements.yml
    
    - src: https://github.com/vantt/ansible_elasticsearch.git
      version: master
      name: elasticsearch_role

How to use
----------

    # playbook.yml
    
    - hosts:  all 
      sudo: yes
      gather_facts: true
      roles:
        - { role: elasticsearch_role }
