typical usage
```
ws   = new Ws_wrap "ws://url"
wsrs = new Wsrs ws
ws_mod_sub ws, wsrs

switch_key = "some_ep"
loc_opt = {
  sub   : {switch : "#{switch_key}_sub"}
  unsub : {switch : "#{switch_key}_unsub"}
  switch: "#{switch_key}_stream"
}
ws.sub loc_opt, (data)->
```
