.. :maxdepth: 2


=======================
Virtualizm installation
=======================

Packages installation
---------------------

.. code-block:: console

    # apt update && apt install virtualizm-api virtualizm-ui

Virtualizm API configuration
----------------------------

Configuration located at **/opt/virtualizm-api/config/app.yml**::


    clusters:
      - id: 1
        name: kvm1
        uri: 'qemu+tls://kvm1.local.domain:16514/system'
        ws_endpoint: 'kvm1.local.domain:8080'
      - id: 2
        name: kvm2
        uri: 'qemu+tls://kvm2.local.domain:16514/system'
        ws_endpoint: 'kvm2.local.domain:8080'
      - id: 3
        name: kvm3
        uri: 'qemu+tls://kvm3.local.domain:16514/system'
        ws_endpoint: 'kvm3.local.domain:8080'

    users:
      - id: 1
        login: demouser
        password: demopassword

    cookie_secret: iHAfQH0gWJB258OhHv69121Qk7YRJcv1XUoGQuh6tPenWvZYKB3qpjgnfggrXurRF64oc4mTHRzwCfSG0P59TPn9YCihzqREfNo2


    cookie_params:
      same_site: 'None'
      secure: true


    # needed to take a screenshot
    libvirt_rw: true
    serve_static: true
    reconnect_timeout: 5
    

    





