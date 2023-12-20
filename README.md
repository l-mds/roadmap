# Local modern Data stack

Vision: Serve as a reference for how the local modern data stack can be used in practice.
Over time build more production grade features and deployment modes to serve as a go-to example for others to spread the use of the software engineering best practices in the LMDS.

items will be checked:

- [ ] to be done
- [x] done

if they are implemented

## batch

the traditional transformations everyone is using

python dependencies with https://github.com/basnijholt/unidep

### ingestion

- https://docs.dagster.io/integrations/embedded-elt

### plain transformation (SQL)

- [ ] dagster
- [ ] duckdb
- [ ] dbt-duckdb
- [ ] excel
- [ ] s3/minio
- [ ] delta lake
- [ ] cube.dev
- [ ] secrets in sops with age

### ML and imperative code

add

- [ ] ray.io, dagaster-pipes
- [ ] simple tabular AI sample

### AI

add
- [ ] LLM case https://github.com/imartinez/privateGPT
    - Qdrant
    - Postgres with pg_vector
- [ ] translation case https://ai.meta.com/resources/models-and-libraries/seamless-communication-models/
- [ ] streaming translation case

## streaming

- dagster
- duckdb
- dbt-duckdb
- s3/minio
- kafka
- risingwave / starrocks
- secrets in sops with age
- some streaming dashboard solution

## open points

to be discussed if we want to include them

- [ ] support multiple deployment modes i.e. local, docker, k8s local via µ-k8s in i.e. rancher desktop, cloud
- [ ] how do lambda functions fit in? In particular ones like: https://modal.com/
- [ ] anomaly detection with dagster stateful asset checks
- [ ] full blown metrics samples based on E2E company tooling mentioned i.e. https://github.com/geoHeil/awesome-tools/blob/master/startup_company.md
- [ ] including commercial PaaS?

## further references

### main
- https://georgheiler.com/2023/12/11/dagster-dbt-duckdb-as-new-local-mds/
- https://juhache.substack.com/p/moving-from-bi-to-data-apps-part?r=l9wvi
- https://www.nintoracaudio.dev/data-eng,music,dx7/2023/12/15/raddd-stack.html
- https://www.infoq.com/news/2023/12/expedia-websockets-kafka-query/
- https://www.youtube.com/watch?v=Nd64jpi-fTE

### background
- https://georgheiler.com/2023/12/01/securing-secrets-with-mozilla-sops-and-age-a-powerful-combo/
- https://georgheiler.com/2022/04/02/making-bigdata-small-again-and-green/
- https://georgheiler.com/2022/04/01/comparing-sql-based-streaming-approaches/
- https://ibrahimhkoyuncu.medium.com/dagster-complete-guide-to-deploy-multiple-data-pipelines-to-dagster-on-kubernetes-environment-b0f83a54fce2