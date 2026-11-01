<img alt="less code · more power — open source · low-code · creator of erupt & linq.j" src="me.svg" width="100%" />

<p align="center">
    <a href="https://www.erupt.xyz"><code><b>[ WEBSITE ]</b></code></a>&nbsp;&nbsp;
    <a href="https://demo.erupt.xyz"><code><b>[ LIVE DEMO ]</b></code></a>&nbsp;&nbsp;
    <a href="https://docs.erupt.xyz"><code><b>[ DOCS ]</b></code></a>&nbsp;&nbsp;
    <a href="https://start.erupt.xyz"><code><b>[ START ]</b></code></a>&nbsp;&nbsp;
    <a href="https://skill.erupt.xyz"><code><b>[ AI SKILL ]</b></code></a>
</p>

<img alt="stack — Low-Code · Big Data · CDP · Data Platform · E-Commerce · Java · Spring · JPA · MySQL · Redis · PostgreSQL · Angular · TypeScript · JavaScript · HTML5 · CSS3 · Spark · Flink · Kafka · ClickHouse · Paimon · Airflow · LLM · Agent · MCP · RAG · AI Coding · Skills · Linux · Docker · K8s · Nginx · Git · Maven · Erupt · Linq.J · Erupt-Web · Erupt-Cube · Erupt-Flow" src="stack.svg" width="100%" />

## `› ls ~/projects`

| PROJECT | WHAT | ★ |
|:--|:--|--:|
| **[erupt](https://github.com/erupts/erupt)** | Code as configuration. Annotate a JPA entity with `@Erupt`, get a production-grade admin backend at runtime — UI, RBAC, audit logs, APIs. No codegen, no frontend. | [![stars](https://img.shields.io/github/stars/erupts/erupt?style=flat-square&label=%E2%98%85&color=ff2a6d&labelColor=0d0221)](https://github.com/erupts/erupt/stargazers) |
| **[erupt‑web](https://github.com/erupts/erupt-web)** | The Angular front end that renders every `@Erupt` entity — the reason you write zero frontend code. | [![stars](https://img.shields.io/github/stars/erupts/erupt-web?style=flat-square&label=%E2%98%85&color=05d9e8&labelColor=0d0221)](https://github.com/erupts/erupt-web/stargazers) |
| **[Linq.J](https://github.com/lambdakit/Linq.J)** | LINQ for Java. Lambda-based object query language on the JVM — `from`, `where`, `groupBy`, `orderBy` over plain collections. | [![stars](https://img.shields.io/github/stars/lambdakit/Linq.J?style=flat-square&label=%E2%98%85&color=f9f002&labelColor=0d0221)](https://github.com/lambdakit/Linq.J/stargazers) |
| **[erupt‑start](https://github.com/erupts/erupt-start)** | Project generator in the browser, like start.spring.io: pick build tool, Java, database and modules, download a ready-to-run ZIP. | `NEW` |
| **[erupt‑cube](https://www.erupt.xyz/#!/cube)** | Semantic layer for billion-row datasets — define metrics once, query them cheaply from any BI. | `PRO` |
| **[erupt‑flow](https://www.erupt.xyz/#!/flow)** | Visual workflow engine: approvals, branches, countersign, all wired to erupt's entities and permissions. | `PRO` |

## `› cat less-code.java`

An admin system is one annotated entity. Add a field, refresh, it shows up — paged, searchable, exportable, role-gated.

```java
@Erupt(name = "User")
@Entity
public class User extends BaseModel {

    @EruptField(
        views = @View(title = "Name"),
        edit  = @Edit(title = "Name", search = @Search)
    )
    private String name = "YuePeng";
}
```

```bash
mvn spring-boot:run        # → http://localhost:8080  (erupt / erupt)
```

No local setup? [start.erupt.xyz](https://start.erupt.xyz) builds the project in your browser. No engineering background? Tell Claude Code `"Build me a CRM admin panel"` with the [erupt skill](https://skill.erupt.xyz) installed.

## `› cat how-i-think.md`

- **Less is more** — the best framework is the one you barely notice.
- **Abstraction over accumulation** — complex problems usually hide a simple model; find it, don't pile code on it.
- **Rewrite without regret** — never married to an implementation, always open to a better one.
- **Ship the runtime, not the generator** — generated code is debt with a nicer name; render from metadata and stay rewritable.

<p align="center"><code>› _</code></p>
