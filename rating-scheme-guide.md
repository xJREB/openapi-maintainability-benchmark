# OpenAPI Rating Scheme

Your task is to analyze each API in this benchmark with respect to its maintainability, i.e. the degree of effectiveness and efficiency with which the underlying system can be modified to correct, improve, extend, or adapt it. Using the [provided schema](rating-scheme.xlsx), you then have to assign four ratings per API, namely ratings for three design properties plus a holistic maintainability score.

Your ratings are based on a relative ordinal scale from `1` to `10`, where, for **all** properties, `10` is the best and `1` is the worst rating. The API that made the most convincing impression on you for a given property will receive a rating of `10` in that category. Each category therefore must have **at least one** rating of `10`. Please rate the other APIs **relative** to the one you rated with the highest score.

We are also very interested in your rationale for these ratings. So for each API and property, there is also a `Comments` field that you can use to briefly document your thought process. This may be especially helpful for very good or very bad ratings, but is nonetheless optional.

## Rating Properties

- **Size:** The volume and breadth of a system. A large system is generally harder to understand and maintain than a small one (provided all other things are similar).

- **Complexity:** The amount, variety, or difficulty of internal work carried out by the system. High complexity makes it difficult to understand the system and has a negative influence on maintainability.

- **Cohesion:** The extent to which the operations of a service contribute towards one task or functionality. A high degree of cohesion positively impacts the maintainability of a service.

- **Overall Maintainability:** A holistic representation of the API's maintainability. You should factor in the previous properties, but you are free to include other aspects of maintainability that you deem important for RESTful APIs and that you can infer from the OpenAPI file. You are also free to assign weights of your judgement to all aspects. This rating can therefore be different from a simple average of the previous three properties. In such a case, we would obviously love some comments on the rationale.

## Final Remarks

- Please remember the relative nature of the benchmark! Even though the API with e.g. the "best" cohesion is still mediocre compared to what you are used to, it still needs to receive a rating of `10`. All other APIs then need to be placed in relation to this API.
- You can include the project in your favourite IDE to ease browsing. You may also use OpenAPI viewing tools like [SwaggerUI](https://swagger.io/tools/swagger-ui), the [Swagger Editor](https://editor.swagger.io), or the [Swagger Viewer VSCode plugin](https://marketplace.visualstudio.com/itemdetails?itemName=Arjun.swagger-viewer).
- Please do not use more sophisticated tool support to analyze the APIs. As mentioned, you may use an IDE or SwaggerUI, but please refrain from using tools like static analyzers. The ratings should be based on your intuitive judgement and personal experience.

**Thank you very much for contributing to this research project! Happy analyzing!**