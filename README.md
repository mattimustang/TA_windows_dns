A Windows DNS debug log Technology Add-on for Splunk that complies with the
Splunk Common Information Model.

To ensure the extractions and `eventtypes work make sure you set the `sourcetype` to `windows:dns`.


Example input configuration:

    [monitor://C:\dns\dns.txt]
    disabled = false
    sourcetype = windows:dns
    # crcSalt required if you are monitoring the file directly on the DNS server
    # as it rotates the log.
    crcSalt = <SOURCE>
