# Why-functions-do-not-work?

Why some functions do not work for ROBLOX exploiting in general?

Reason 1: **The offsets are not updated**, or at least one of them.
- Functions like pushboolean need an address and a working convention to run, otherwise CRASH.
- A function can have *more then one offset*, so maybe the other ones are not updated.
- How to fix?: Simply just *update the offsets*. Yeah that easy. I was amazed when i used to be n00b.


Reason 2: **DWORD and Lua_State are Waayyyy Different stuff?**
- lua_state is like DWORD but included inside of the lua 5.1 library. DWORD is an int, if you think about it.
- Scanning codes are like *DWORD rob = Scan(blah, blah, 0, NULL, blah)*, but the lua_state was never included.
- To change, replace *DWORD* with the lua_State* method or you can just pass the scan to the DWORD or lua_state.
- How to fix?: Passing to other: rob = lua; (where lua is lua_state and rob is DWORD), ez.


Reason 3: your a big skid and dont know any C++ just knows including but even a 6 year old can do that)
