## What Google Learned From Its Quest to Build the Perfect Team
Project Aristotle’s researchers began by reviewing a half-century of academic studies looking at how teams worked. Were the best teams made up of people with similar interests? Or did it matter more whether everyone was motivated by the same kinds of rewards? Based on those studies, the researchers scrutinized the composition of groups inside Google: How often did teammates socialize outside the office? Did they have the same hobbies? Were their educational backgrounds similar? Was it better for all teammates to be outgoing or for all of them to be shy? They drew diagrams showing which teams had overlapping memberships and which groups had exceeded their departments’ goals.

## SuperAgent
SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!

> Request basics :

- A request can be initiated by invoking the appropriate method on the request object, then calling ``.then()`` (or ``.end()`` or ``await``) to send the request. For example a simple GET request
- DELETE can be also called as ``.del()`` for compatibility with old IE where delete is a reserved word.
- Setting header fields is simple, invoke ``.set()`` with a field name and value
- The ``.query()`` method accepts objects, which when used with the GET method will form a query-string. The following will produce the path /search?query=Manny&range=1..5&order=desc.
- By default sending strings will set the Content-Type to ``application/x-www-form-urlencoded``, multiple calls will be concatenated with ``&``, here resulting in ``name=tj&pet=tobi``

>Agents for global state
- In Node SuperAgent does not save cookies by default, but you can use the ``.agent()`` method to create a copy of SuperAgent that saves cookies.
- he complete list of methods that the agent can use to set defaults is: ``use``, ``on``, ``once``, ``set``, ``query``, ``type``, ``accept``, ``auth``, ``withCredentials``, ``sortQuery``, ``retry``, ``ok``, ``redirects``, ``timeout``, ``buffer``, ``serializ``, ``parse``, ``ca``,``key``, ``pfx``, ``cert.``

>Piping data
- The Node client allows you to pipe data to and from the request. Please note that ``.pipe()`` is used instead of ``.end()/.then()`` methods.

>Progress tracking
- SuperAgent fires ``progress`` events on upload and download of large files.

>Ignoring broken/insecure HTTPS on localhost
- In Node.js, when HTTPS is misconfigured and insecure (e.g. using self-signed certificate without specifying own .ca()), it's still possible to permit requests to localhost by calling ``.trustLocalhost()``
> Promise and Generator support
- SuperAgent's request is a "thenable" object that's compatible with JavaScript promises and the ``async/await`` syntax.

>Browser and node versions
- Electron developers report if you would prefer to use the browser version of SuperAgent instead of the Node version, you can require``('superagent/superagent')``. Your requests will now show up in the Chrome developer tools Network tab. Note this environment is not covered by automated test suite and not officially supported.

