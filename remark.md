记录此项目的思考

# 分析token消耗过快的处理方案
client.token.usage接入Prometheus
localhost:8080/actuator/metrics/gen_ai.client.token.usage 。该指标集成由强大的 Micrometer 项目提供支持，该项目几乎可以与所有主流时间序列数据库集成，包括 Prometheus
可以监控token消耗，什么情况下告警。一般监控到token消耗过快如何处理？
