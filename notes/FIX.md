To protect your web application from insecure deserialization, it is crucial never to pass a serialized object manipulated with untrusted input by the user to the deserialize function. The reason is that if you do so, an untrusted user would be able to manipulate the object and can send it directly to the Python deserialize function.


- Introduce digital signatures and other integrity checks to stop malicious object creation or other data interfering.
- Run deserialization code in low privilege environments.
- Keep a log with deserialization exceptions and failures.
- Execute strict constraints for the deserialization processes before object creation.
- Limit and check all incoming and outgoing network activity from deserialization containers and servers.
- Keep tabs on deserialization activities to identify in case there is constant deserialization by a user.
- Use deserialization methods like JSON, XML, and YAML that are language-agnostic.
