licenses(["notice"])  # Apache 2

package_group(
    name = "docs",
    packages = [
        "//docs",
    ],
)

# TODO(htuch): Grow this to cover everything we want to generate docs for, so we can just invoke
# bazel build //docs:protos --aspects tools/protodoc/protodoc.bzl%proto_doc_aspect  --output_groups=rst
proto_library(
    name = "protos",
    deps = [
        "//envoy/api/v2:cds",
        "//envoy/api/v2:discovery",
        "//envoy/api/v2:eds",
        "//envoy/api/v2:lds",
        "//envoy/api/v2:rds",
        "//envoy/api/v2/cluster:circuit_breaker",
        "//envoy/api/v2/cluster:outlier_detection",
        "//envoy/api/v2/core:protocol",
        "//envoy/api/v2/listener",
        "//envoy/api/v2/ratelimit",
        "//envoy/api/v2/route",
        "//envoy/config/bootstrap/v2:bootstrap",
        "//envoy/config/filter/accesslog/v2:accesslog",
        "//envoy/config/filter/http/buffer/v2:buffer",
        "//envoy/config/filter/http/ext_authz/v2:ext_authz",
        "//envoy/config/filter/http/fault/v2:fault",
        "//envoy/config/filter/http/gzip/v2:gzip",
        "//envoy/config/filter/http/health_check/v2:health_check",
        "//envoy/config/filter/http/lua/v2:lua",
        "//envoy/config/filter/http/rate_limit/v2:rate_limit",
        "//envoy/config/filter/http/router/v2:router",
        "//envoy/config/filter/http/squash/v2:squash",
        "//envoy/config/filter/http/transcoder/v2:transcoder",
        "//envoy/config/filter/network/client_ssl_auth/v2:client_ssl_auth",
        "//envoy/config/filter/network/ext_authz/v2:ext_authz",
        "//envoy/config/filter/network/http_connection_manager/v2:http_connection_manager",
        "//envoy/config/filter/network/mongo_proxy/v2:mongo_proxy",
        "//envoy/config/filter/network/rate_limit/v2:rate_limit",
        "//envoy/config/filter/network/redis_proxy/v2:redis_proxy",
        "//envoy/config/filter/network/tcp_proxy/v2:tcp_proxy",
        "//envoy/config/metrics/v2:metrics_service",
        "//envoy/config/metrics/v2:stats",
        "//envoy/config/ratelimit/v2:rls",
        "//envoy/config/trace/v2:trace",
        "//envoy/service/discovery/v2:ads",
        "//envoy/service/load_stats/v2:lrs",
        "//envoy/service/metrics/v2:metrics_service",
    ],
)
