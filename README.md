# Y collective
> A transparent funding organization that finances the work on open-source tools for creating collaborative & decentralized applications - https://opencollective.com/y-collective

We want to improve the ecosystem around the [Yjs CRDT](https://github.com/yjs/yjs) for building collaborative applications. The y-collective is managed by trusted authors of relevant software libraries in this space. We define the work that this collective is funding based on the interest of our sponsors. The maintainers of approved projects can charge up to $100/h for approved work and must make their timesheets publically available.

Please use the [discussion board](https://github.com/y-community/y-collective/discussions) to ask questions or to provide feedback.

## Members

* Kevin Jahns ([Yjs](https://github.com/yjs/yjs))
* Hans Pagel ([Hocuspocus](https://www.hocuspocus.dev)
* Philipp Kühn ([Tiptap](https://github.com/ueberdosis/tiptap))

## Projects

In this section we define the work that y-collective is funding. If you want to make a significant contribution to work that is not listed here, then please contact us directly so we can define the work together. 

### Hocuspocus
> [Hocuspocus](https://www.hocuspocus.dev/) is an extensible, infinitely scalable server for Yjs documents. 

* Extension interface for custom authentication mechanisms.
* Extension interface for storing the shared document in a central database for indexing and persistence.
* Work on [y-redis](https://github.com/yjs/y-redis/) as a provider for infinite scalability.
* Support for efficient synchronization of [Yjs' subdocuments](https://docs.yjs.dev/api/subdocuments).

##### Gold Sponsors: 

<a href="https://cargo.site/"><img height="70" alt="cargo" src="https://user-images.githubusercontent.com/5553757/118843640-8a696680-b8ca-11eb-9b5b-9e53c5d7c5a7.png"></a>

<a href="https://saga.so/"><img height="70" alt="saga-logo" src="https://user-images.githubusercontent.com/5553757/118843142-0f07b500-b8ca-11eb-9418-1dd9505b0e8d.png"></a>

### Y-CRDT
> [Y-CRDT](https://github.com/yjs/y-crdt) is a port of the Yjs CRDT to different languages.

Our goal is to make the Y CRDT ubiquitious by providing ports of Yjs to many different languages like Swift, Go, WASM, PHP, Python, Java, ..

We already started the work on Yrs ("wires") - a high-performance port of the Yjs CRDT to the Rust programming language. We are working on novel data structures to represent the internal CRDT structure even more efficiently than Yjs. Once we have a reference implementation, we will port Yrs to different languages using language bindings. 

* Yrs - Work on a full port of the Yjs CRDT to the Rust programming language.
  * Find appropriate data structures to represent the CRDT structures in Rust.
  * Sync with Yjs documents (implement the updates API https://docs.yjs.dev/api/document-updates#update-api).
  * Read the Yjs documents (implement shared types including the API to read the content. It will be possible to convert the types to a JSON representation).
  * Functionality to manipulate shared types (Y.Map and Y.Array will be fully implemented. But Y.Text won't implement the complete extensive rich-text API).
  * Publish a Yrs cargo package including documentation
  * Performance analysis compared to Yjs and Automerge
* Provide WASM bindings (see [Ywasm](https://github.com/yjs/y-crdt/tree/main/ywasm))
  * Performance analysis compared to Yjs and Automerge
* Provide Python bindings (see [Ypy](https://github.com/yjs/y-crdt/tree/main/y-py))

### Tiptap
> [Tiptap](https://www.tiptap.dev/) is a headless editor framework, with core support for collaborative editing.


