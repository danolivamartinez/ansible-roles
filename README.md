roles/config-agent
==========

Rol con el servicio config-agent.

configura una ec2 con capacidad de inventario dinamico para desplegar playbook


Requirements
------------

None

Role Variables
--------------

| Variable   | Descripcion                                 | Requerida  | Valores        |
| ---------- | ------------------------------------------- | ---------- | -------------- |
| env        | Entorno de la cuenta                        | Sí, CI/CD  | prod, nonprod  |
| aws_region | Region de AWS donde se crea la imagen       | Sí, CI/CD  | eu-west-1, ... |
| config_agent_user | usuario que usa torre para para conectar al agente       | Sí, CI/CD  | ansible |
| deploy_user | usuario con el que se conectara en agente para configurar las ec2       | Sí, CI/CD  | ec2-user |

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - config-agent


License
-------

All Rights Reserved. Orange Espagne, 2019

Author Information
------------------

OSP CoE Cloud <ld.coecloud@orange.com>
