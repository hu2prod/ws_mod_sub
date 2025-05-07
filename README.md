typical usage
```
ws   = new Ws_wrap "ws://url"
wsrs = new Wsrs ws
ws_mod_sub ws, wsrs

switch_key = "some_ep"
ws.sub {
  sub   : obj_set {switch : "#{switch_key}_sub"}, opt
  unsub : obj_set {switch : "#{switch_key}_unsub"}, opt
  switch: "#{switch_key}_stream"
}
```
