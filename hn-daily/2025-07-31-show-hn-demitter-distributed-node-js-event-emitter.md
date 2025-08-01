# Show HN: Demitter – Distributed Node.js Event Emitter (Pub/Sub)

**Posted by pmbanugo on 2025-07-31**

---

What if you could turn Node.js's event emitter into a distributed pub-sub system?

I built Demitter to address a recurring challenge: how to easily share events between Node.js processes without the complexity of setting up heavyweight message brokers like Redis or RabbitMQ. It uses ZeroMQ for messaging and MessagePack for serialization, ensuring high performance even under high event loads.

### What Demitter does:
- Provides the familiar `emitter.on()` and `emitter.emit()` APIs you already know in Node.js.
- Seamlessly works across multiple processes and machines.
- Requires zero configuration: just `npm install demitter` and you're ready to go.

### See it in action:
I created a live auction demo where multiple bidders run in separate terminal windows, all bidding in real-time on the same auctions. Watch it here: [YouTube demo](https://www.youtube.com/watch?v=LqQShQ9-dsk). It's quite satisfying to see around 7 processes stay perfectly synchronized in real-time.

### Use cases:
- Coordinating worker processes without added complexity.
- Scaling Socket.IO or WebSocket servers without relying on heavy message brokers.
- Any other scenario requiring pub/sub across Node.js processes.

I developed Demitter because I wanted a lightweight solution that retained the familiar Node.js event API. Existing solutions felt too heavy for simple pub/sub needs, and I wanted to keep the API developers already know.

---

I'd love to hear your thoughts. Do you see this being useful? What other use cases do you think it could solve for you?

I'm in the EU, and it's very late here, so I’ll catch up on comments tomorrow.