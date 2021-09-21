## v0.0.6 (2021-09-21)

* return a variant from timer to indicate whether there are connections pending
  or the timer can be suspended -- this avoids unnecessary busy work (@reynir)
* connect_ip: take list of Ipaddr.t and int pairs instead of separate lists.
  The reason for this change is the dns-client. (@hannesm @reynir)

## v0.0.5 (2021-09-13)

* connect_ip: take an optional shuffle argument and an ordered list of ips to
  attempt connections to. The reason for this change is that /etc/resolv.conf
  specifies an ordering. (@hannesm)

## v0.0.4 (2021-09-11)

* Use set from ipaddr (>= 5.2.0) instead providing these (@hannesm)

## v0.0.3 (2021-09-07)

* BUGFIX: Avoid exception if expand_list is called with an empty list (@hannesm)

## v0.0.2 (2021-09-06)

* BUGFIX: Delay connect failure if v6 resolution and connection attempt fails
  before v4 resolution had a chance to succeed or fail (issue #9). (@hannesm)

## v0.0.1 (2021-08-24)

* Initial release (@hannesm)
