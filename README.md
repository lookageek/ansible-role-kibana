# Ansible Role: Kibana

An Ansible Role that installs Kibana on Debian/Ubuntu with systemd.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    elasticstack_deb_repo: "5.x"

The elasticstack debian repo version

    kibana_version: "5.3.2"

Specific kibana version to install

    kibana_enabled_on_boot: yes

Set this to `no` if you don't want kibana to run on system startup.

    kibana_server_port: 5601
    kibana_server_host: "0.0.0.0"

The FQDN or IP address and port Kibana should use.

    kibana_elasticsearch_url: "http://localhost:9200"

The URL (including port) over which Kibana will connect to Elasticsearch.

## Dependencies

None.

## License

MIT / BSD

## Author Information

This role was created in 2017 by Jayanth Manklu cloning from [geerlingguy/ansible-role-kibana](https://github.com/geerlingguy/ansible-role-kibana).
