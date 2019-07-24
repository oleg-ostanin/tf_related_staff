cmake_minimum_required(VERSION 3.14)
project(tensorflow)

set(CMAKE_CXX_STANDARD 14)

include_directories(/home/oostanin/tf_related_repos/abseil-cpp)
include_directories(/home/oostanin/tf_related_repos/protobuf/src/)

include_directories(/home/oostanin/tensorflow)
include_directories(/home/oostanin/tensorflow/bazel-genfiles)

file(GLOB tensorflow_contrib_tensorrt_shape_fn "${CMAKE_SOURCE_DIR}/tensorflow/contrib/tensorrt/shape_fn/*.cc")
file(GLOB tensorflow_compiler_xla_service_llvm_ir "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/service/llvm_ir/*.cc")
file(GLOB tensorflow_lite_delegates_gpu_gl "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/gl/*.cc")
file(GLOB tensorflow_lite_tools_benchmark_android_jni "${CMAKE_SOURCE_DIR}/tensorflow/lite/tools/benchmark/android/jni/*.cc")
file(GLOB tensorflow_compiler_xrt_client "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xrt/client/*.cc")
file(GLOB tensorflow_contrib_periodic_resample_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/periodic_resample/ops/*.cc")
file(GLOB tensorflow_core_grappler_utils "${CMAKE_SOURCE_DIR}/tensorflow/core/grappler/utils/*.cc")
file(GLOB tensorflow_lite_experimental_ruy "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/ruy/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_eigen3 "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/btl/libs/eigen3/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_eigen2 "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/btl/libs/eigen2/*.cc")
file(GLOB tensorflow_lite_tools_accuracy_ilsvrc "${CMAKE_SOURCE_DIR}/tensorflow/lite/tools/accuracy/ilsvrc/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_demos_mandelbrot "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/demos/mandelbrot/*.cc")
file(GLOB tensorflow_core_kernels_rnn "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/rnn/*.cc")
file(GLOB tensorflow_core_profiler_internal "${CMAKE_SOURCE_DIR}/tensorflow/core/profiler/internal/*.cc")
file(GLOB tensorflow_c_kernels "${CMAKE_SOURCE_DIR}/tensorflow/c/kernels/*.cc")
file(GLOB tensorflow_core_nccl "${CMAKE_SOURCE_DIR}/tensorflow/core/nccl/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_blitz "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/btl/libs/blitz/*.cc")
file(GLOB tensorflow_contrib_ignite_kernels_igfs "${CMAKE_SOURCE_DIR}/tensorflow/contrib/ignite/kernels/igfs/*.cc")
file(GLOB tensorflow_core_grappler "${CMAKE_SOURCE_DIR}/tensorflow/core/grappler/*.cc")
file(GLOB tensorflow_lite_models_smartreply "${CMAKE_SOURCE_DIR}/tensorflow/lite/models/smartreply/*.cc")
file(GLOB tensorflow_lite_tools_evaluation_stages "${CMAKE_SOURCE_DIR}/tensorflow/lite/tools/evaluation/stages/*.cc")
file(GLOB tensorflow_core_util_ctc "${CMAKE_SOURCE_DIR}/tensorflow/core/util/ctc/*.cc")
file(GLOB tensorflow_examples_speech_commands "${CMAKE_SOURCE_DIR}/tensorflow/examples/speech_commands/*.cc")
file(GLOB tensorflow_contrib_boosted_trees_lib_quantiles "${CMAKE_SOURCE_DIR}/tensorflow/contrib/boosted_trees/lib/quantiles/*.cc")
file(GLOB tensorflow_core_distributed_runtime "${CMAKE_SOURCE_DIR}/tensorflow/core/distributed_runtime/*.cc")
file(GLOB tensorflow_core_kernels_tensor_forest "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/tensor_forest/*.cc")
file(GLOB tensorflow_lite_models_smartreply_ops "${CMAKE_SOURCE_DIR}/tensorflow/lite/models/smartreply/ops/*.cc")
file(GLOB tensorflow_lite_models_smartreply_demo_app_src_main "${CMAKE_SOURCE_DIR}/tensorflow/lite/models/smartreply/demo/app/src/main/*.cc")
file(GLOB tensorflow_lite_tools_benchmark "${CMAKE_SOURCE_DIR}/tensorflow/lite/tools/benchmark/*.cc")
file(GLOB tensorflow_contrib_layers_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/layers/kernels/*.cc")
file(GLOB tensorflow_compiler_aot_tests "${CMAKE_SOURCE_DIR}/tensorflow/compiler/aot/tests/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_gmm "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/btl/libs/gmm/*.cc")
file(GLOB tensorflow_lite_delegates_gpu_gl_kernels "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/gl/kernels/*.cc")
file(GLOB tensorflow_stream_executor_platform_default "${CMAKE_SOURCE_DIR}/tensorflow/stream_executor/platform/default/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_BLAS "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/btl/libs/BLAS/*.cc")
file(GLOB tensorflow_stream_executor_gpu "${CMAKE_SOURCE_DIR}/tensorflow/stream_executor/gpu/*.cc")
file(GLOB third_party_toolchains_preconfig_centos6_gcc7_tools_cpp "${CMAKE_SOURCE_DIR}/third_party/toolchains/preconfig/centos6/gcc7/tools/cpp/*.cc")
file(GLOB tensorflow_lite_delegates_gpu_java_src_main_native "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/java/src/main/native/*.cc")
file(GLOB tensorflow_core_summary "${CMAKE_SOURCE_DIR}/tensorflow/core/summary/*.cc")
file(GLOB tensorflow_contrib_hadoop_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/hadoop/ops/*.cc")
file(GLOB tensorflow_lite_delegates_gpu_metal_kernels "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/metal/kernels/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_perf_monitoring "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/perf_monitoring/*.cc")
file(GLOB tensorflow_core_lib_io_snappy "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/io/snappy/*.cc")
file(GLOB tensorflow_contrib_tensor_forest_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/tensor_forest/ops/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_speech_simple_features "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_speech/simple_features/*.cc")
file(GLOB tensorflow_core_util_proto "${CMAKE_SOURCE_DIR}/tensorflow/core/util/proto/*.cc")
file(GLOB tensorflow_core_lib_random "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/random/*.cc")
file(GLOB tensorflow_contrib_kafka_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/kafka/kernels/*.cc")
file(GLOB tensorflow_compiler_tests "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tests/*.cc")
file(GLOB tensorflow_contrib_android "${CMAKE_SOURCE_DIR}/tensorflow/contrib/android/*.cc")
file(GLOB tensorflow_core_profiler "${CMAKE_SOURCE_DIR}/tensorflow/core/profiler/*.cc")
file(GLOB tensorflow_cc_tutorials "${CMAKE_SOURCE_DIR}/tensorflow/cc/tutorials/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_blas "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/blas/*.cc")
file(GLOB tensorflow_contrib_boosted_trees_lib_trees "${CMAKE_SOURCE_DIR}/tensorflow/contrib/boosted_trees/lib/trees/*.cc")
file(GLOB tensorflow_core_kernels_data "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/data/*.cc")
file(GLOB tensorflow_lite_toco_tensorflow_graph_matching "${CMAKE_SOURCE_DIR}/tensorflow/lite/toco/tensorflow_graph_matching/*.cc")
file(GLOB tensorflow_contrib_session_bundle "${CMAKE_SOURCE_DIR}/tensorflow/contrib/session_bundle/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_speech "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_speech/*.cc")
file(GLOB tensorflow_python_client "${CMAKE_SOURCE_DIR}/tensorflow/python/client/*.cc")
file(GLOB tensorflow_compiler_mlir_tensorflow_ir "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/tensorflow/ir/*.cc")
file(GLOB tensorflow_contrib_bigtable_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/bigtable/ops/*.cc")
file(GLOB tensorflow_lite_schema "${CMAKE_SOURCE_DIR}/tensorflow/lite/schema/*.cc")
file(GLOB tensorflow_contrib_pi_examples_label_image "${CMAKE_SOURCE_DIR}/tensorflow/contrib/pi_examples/label_image/*.cc")
file(GLOB tensorflow_stream_executor_rocm "${CMAKE_SOURCE_DIR}/tensorflow/stream_executor/rocm/*.cc")
file(GLOB tensorflow_contrib_tensor_forest_hybrid_core_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/tensor_forest/hybrid/core/ops/*.cc")
file(GLOB tensorflow_core_lib_db "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/db/*.cc")
file(GLOB tensorflow_contrib_hvx_clock_cycle_profiling "${CMAKE_SOURCE_DIR}/tensorflow/contrib/hvx/clock_cycle_profiling/*.cc")
file(GLOB tensorflow_lite_examples_label_image "${CMAKE_SOURCE_DIR}/tensorflow/lite/examples/label_image/*.cc")
file(GLOB tensorflow_core_lib_wav "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/wav/*.cc")
file(GLOB tensorflow_java_src_gen_cc "${CMAKE_SOURCE_DIR}/tensorflow/java/src/gen/cc/*.cc")
file(GLOB tensorflow_contrib_boosted_trees_lib_utils "${CMAKE_SOURCE_DIR}/tensorflow/contrib/boosted_trees/lib/utils/*.cc")
file(GLOB tensorflow_compiler_mlir_lite_python "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/lite/python/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_gemmlowp_meta "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/gemmlowp/meta/*.cc")
file(GLOB tensorflow_contrib_pi_examples_camera "${CMAKE_SOURCE_DIR}/tensorflow/contrib/pi_examples/camera/*.cc")
file(GLOB tensorflow_python_grappler "${CMAKE_SOURCE_DIR}/tensorflow/python/grappler/*.cc")
file(GLOB tensorflow_cc_saved_model "${CMAKE_SOURCE_DIR}/tensorflow/cc/saved_model/*.cc")
file(GLOB tensorflow_contrib_tpu_profiler "${CMAKE_SOURCE_DIR}/tensorflow/contrib/tpu/profiler/*.cc")
file(GLOB tensorflow_core_util_rpc "${CMAKE_SOURCE_DIR}/tensorflow/core/util/rpc/*.cc")
file(GLOB tensorflow_core_grappler_graph_analyzer "${CMAKE_SOURCE_DIR}/tensorflow/core/grappler/graph_analyzer/*.cc")
file(GLOB tensorflow_core_lib_hash "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/hash/*.cc")
file(GLOB tensorflow_compiler_jit "${CMAKE_SOURCE_DIR}/tensorflow/compiler/jit/*.cc")
file(GLOB tensorflow_python_eager "${CMAKE_SOURCE_DIR}/tensorflow/python/eager/*.cc")
file(GLOB tensorflow_core_platform_profile_utils "${CMAKE_SOURCE_DIR}/tensorflow/core/platform/profile_utils/*.cc")
file(GLOB tensorflow_tools_proto_text "${CMAKE_SOURCE_DIR}/tensorflow/tools/proto_text/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_spbench "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/spbench/*.cc")
file(GLOB tensorflow_contrib_libsvm_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/libsvm/ops/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_speech_CMSIS "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_speech/CMSIS/*.cc")
file(GLOB tensorflow_compiler_xrt_ops "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xrt/ops/*.cc")
file(GLOB tensorflow_contrib_factorization_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/factorization/ops/*.cc")
file(GLOB tensorflow_lite_tools_accuracy "${CMAKE_SOURCE_DIR}/tensorflow/lite/tools/accuracy/*.cc")
file(GLOB tensorflow_core_debug "${CMAKE_SOURCE_DIR}/tensorflow/core/debug/*.cc")
file(GLOB tensorflow_tools_ci_build_builds_user_ops "${CMAKE_SOURCE_DIR}/tensorflow/tools/ci_build/builds/user_ops/*.cc")
file(GLOB tensorflow_core_platform_cloud "${CMAKE_SOURCE_DIR}/tensorflow/core/platform/cloud/*.cc")
file(GLOB tensorflow_contrib_cloud_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/cloud/kernels/*.cc")
file(GLOB tensorflow_compiler_xla_service_gpu_llvm_gpu_backend "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/service/gpu/llvm_gpu_backend/*.cc")
file(GLOB tensorflow_compiler_mlir_tensorflow_translate "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/tensorflow/translate/*.cc")
file(GLOB tensorflow_java "${CMAKE_SOURCE_DIR}/tensorflow/java/*.cc")
file(GLOB tensorflow_lite_kernels_internal_reference "${CMAKE_SOURCE_DIR}/tensorflow/lite/kernels/internal/reference/*.cc")
file(GLOB tensorflow_contrib_cloud_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/cloud/ops/*.cc")
file(GLOB tensorflow_contrib_nearest_neighbor_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/nearest_neighbor/ops/*.cc")
file(GLOB tensorflow_cc_training "${CMAKE_SOURCE_DIR}/tensorflow/cc/training/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_vision_sparkfun_edge "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_vision/sparkfun_edge/*.cc")
file(GLOB tensorflow_contrib_image_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/image/kernels/*.cc")
file(GLOB tensorflow_core_platform_hadoop "${CMAKE_SOURCE_DIR}/tensorflow/core/platform/hadoop/*.cc")
file(GLOB tensorflow_contrib_text_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/text/ops/*.cc")
file(GLOB tensorflow_contrib_input_pipeline_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/input_pipeline/ops/*.cc")
file(GLOB tensorflow_compiler_tf2xla_ops "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2xla/ops/*.cc")
file(GLOB tensorflow_lite_examples_minimal "${CMAKE_SOURCE_DIR}/tensorflow/lite/examples/minimal/*.cc")
file(GLOB tensorflow_compiler_mlir_xla_ir "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/xla/ir/*.cc")
file(GLOB tensorflow_core_kernels_hexagon "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/hexagon/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_test "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/test/*.cc")
file(GLOB tensorflow_java_src_test_native "${CMAKE_SOURCE_DIR}/tensorflow/java/src/test/native/*.cc")
file(GLOB tensorflow_lite_experimental_c "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/c/*.cc")
file(GLOB tensorflow_lite_tools_optimize_calibration "${CMAKE_SOURCE_DIR}/tensorflow/lite/tools/optimize/calibration/*.cc")
file(GLOB tensorflow_contrib_cmake_tests_cuda "${CMAKE_SOURCE_DIR}/tensorflow/contrib/cmake/tests/cuda/*.cc")
file(GLOB tensorflow_compiler_xla_python "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/python/*.cc")
file(GLOB tensorflow_compiler_xla_client "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/client/*.cc")
file(GLOB tensorflow_core_kernels_neon "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/neon/*.cc")
file(GLOB tensorflow_lite_c "${CMAKE_SOURCE_DIR}/tensorflow/lite/c/*.cc")
file(GLOB tensorflow_lite_experimental_micro_mbed "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/mbed/*.cc")
file(GLOB tensorflow_compiler_mlir_lite_tools "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/lite/tools/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_gemmlowp_doc "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/gemmlowp/doc/*.cc")
file(GLOB tensorflow_compiler_tf2xla_lib "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2xla/lib/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_hello_world "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/hello_world/*.cc")
file(GLOB tensorflow_lite_profiling "${CMAKE_SOURCE_DIR}/tensorflow/lite/profiling/*.cc")
file(GLOB tensorflow_contrib_bigtable_kernels_test_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/bigtable/kernels/test_kernels/*.cc")
file(GLOB tensorflow_contrib_gdr "${CMAKE_SOURCE_DIR}/tensorflow/contrib/gdr/*.cc")
file(GLOB tensorflow_lite_tools_evaluation_stages_utils "${CMAKE_SOURCE_DIR}/tensorflow/lite/tools/evaluation/stages/utils/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_hello_world_disco_f746ng "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/hello_world/disco_f746ng/*.cc")
file(GLOB tensorflow_core_distributed_runtime_rpc_eager "${CMAKE_SOURCE_DIR}/tensorflow/core/distributed_runtime/rpc/eager/*.cc")
file(GLOB tensorflow_examples_android_jni_object_tracking "${CMAKE_SOURCE_DIR}/tensorflow/examples/android/jni/object_tracking/*.cc")
file(GLOB tensorflow_compiler_jit_tests "${CMAKE_SOURCE_DIR}/tensorflow/compiler/jit/tests/*.cc")
file(GLOB tensorflow_core_profiler_lib "${CMAKE_SOURCE_DIR}/tensorflow/core/profiler/lib/*.cc")
file(GLOB tensorflow_contrib_kafka_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/kafka/ops/*.cc")
file(GLOB tensorflow_contrib_mpi "${CMAKE_SOURCE_DIR}/tensorflow/contrib/mpi/*.cc")
file(GLOB tensorflow_tools_benchmark "${CMAKE_SOURCE_DIR}/tensorflow/tools/benchmark/*.cc")
file(GLOB tensorflow_java_src_main_native "${CMAKE_SOURCE_DIR}/tensorflow/java/src/main/native/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_speech_simple_features_CMSIS "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_speech/simple_features/CMSIS/*.cc")
file(GLOB cmake-build-debug_CMakeFiles_3.14.3_CompilerIdCXX "${CMAKE_SOURCE_DIR}/cmake-build-debug/CMakeFiles/3.14.3/CompilerIdCXX/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_speech_micro_features "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_speech/micro_features/*.cc")
file(GLOB tensorflow_compiler_xla_rpc "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/rpc/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_unsupported_test "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/unsupported/test/*.cc")
file(GLOB tensorflow_core_grappler_costs "${CMAKE_SOURCE_DIR}/tensorflow/core/grappler/costs/*.cc")
file(GLOB tensorflow_compiler_mlir_tensorflow_transforms "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/tensorflow/transforms/*.cc")
file(GLOB tensorflow_c_experimental "${CMAKE_SOURCE_DIR}/tensorflow/c/experimental/*.cc")
file(GLOB tensorflow_compiler_mlir_lite_ir "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/lite/ir/*.cc")
file(GLOB tensorflow_core_common_runtime_eager "${CMAKE_SOURCE_DIR}/tensorflow/core/common_runtime/eager/*.cc")
file(GLOB tensorflow_examples_android_jni "${CMAKE_SOURCE_DIR}/tensorflow/examples/android/jni/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_blaze "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/btl/libs/blaze/*.cc")
file(GLOB tensorflow_lite_experimental_micro_bluepill "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/bluepill/*.cc")
file(GLOB tensorflow_contrib_seq2seq_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/seq2seq/ops/*.cc")
file(GLOB tensorflow_lite_experimental_micro_kernels "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/kernels/*.cc")
file(GLOB tensorflow_contrib_resampler_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/resampler/ops/*.cc")
file(GLOB tensorflow_contrib_fused_conv_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/fused_conv/ops/*.cc")
file(GLOB tensorflow_core_kernels_boosted_trees_quantiles "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/boosted_trees/quantiles/*.cc")
file(GLOB tensorflow_lite_experimental_micro_chre "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/chre/*.cc")
file(GLOB tensorflow_compiler_xla_service "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/service/*.cc")
file(GLOB tensorflow_lite_experimental_micro_arduino "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/arduino/*.cc")
file(GLOB tensorflow_contrib_mpi_collectives "${CMAKE_SOURCE_DIR}/tensorflow/contrib/mpi_collectives/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_speech_sparkfun_edge "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_speech/sparkfun_edge/*.cc")
file(GLOB tensorflow_lite_experimental_micro_kernels_cmsis-nn "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/kernels/cmsis-nn/*.cc")
file(GLOB tensorflow_core_distributed_runtime_rpc "${CMAKE_SOURCE_DIR}/tensorflow/core/distributed_runtime/rpc/*.cc")
file(GLOB tensorflow_examples_adding_an_op "${CMAKE_SOURCE_DIR}/tensorflow/examples/adding_an_op/*.cc")
file(GLOB tensorflow_cc_gradients "${CMAKE_SOURCE_DIR}/tensorflow/cc/gradients/*.cc")
file(GLOB tensorflow_contrib_framework_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/framework/kernels/*.cc")
file(GLOB tensorflow_python_framework "${CMAKE_SOURCE_DIR}/tensorflow/python/framework/*.cc")
file(GLOB tensorflow_core_common_runtime_sycl "${CMAKE_SOURCE_DIR}/tensorflow/core/common_runtime/sycl/*.cc")
file(GLOB tensorflow_core_util "${CMAKE_SOURCE_DIR}/tensorflow/core/util/*.cc")
file(GLOB tensorflow_core_profiler_rpc "${CMAKE_SOURCE_DIR}/tensorflow/core/profiler/rpc/*.cc")
file(GLOB tensorflow_lite_delegates_nnapi "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/nnapi/*.cc")
file(GLOB tensorflow_lite_models "${CMAKE_SOURCE_DIR}/tensorflow/lite/models/*.cc")
file(GLOB tensorflow_lite_nnapi "${CMAKE_SOURCE_DIR}/tensorflow/lite/nnapi/*.cc")
file(GLOB tensorflow_lite_toco_graph_transformations "${CMAKE_SOURCE_DIR}/tensorflow/lite/toco/graph_transformations/*.cc")
file(GLOB tensorflow_compiler_jit_ops "${CMAKE_SOURCE_DIR}/tensorflow/compiler/jit/ops/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_unsupported_doc_examples "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/unsupported/doc/examples/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_hello_world_arduino "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/hello_world/arduino/*.cc")
file(GLOB tensorflow_core_grappler_verifiers "${CMAKE_SOURCE_DIR}/tensorflow/core/grappler/verifiers/*.cc")
file(GLOB tensorflow_contrib_android_jni "${CMAKE_SOURCE_DIR}/tensorflow/contrib/android/jni/*.cc")
file(GLOB tensorflow_lite_kernels_internal_optimized "${CMAKE_SOURCE_DIR}/tensorflow/lite/kernels/internal/optimized/*.cc")
file(GLOB tensorflow_contrib_verbs "${CMAKE_SOURCE_DIR}/tensorflow/contrib/verbs/*.cc")
file(GLOB tensorflow_lite_experimental_microfrontend_lib "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/microfrontend/lib/*.cc")
file(GLOB tensorflow_core_common_runtime_gpu "${CMAKE_SOURCE_DIR}/tensorflow/core/common_runtime/gpu/*.cc")
file(GLOB tensorflow_contrib_ignite_kernels_dataset "${CMAKE_SOURCE_DIR}/tensorflow/contrib/ignite/kernels/dataset/*.cc")
file(GLOB tensorflow_compiler_aot "${CMAKE_SOURCE_DIR}/tensorflow/compiler/aot/*.cc")
file(GLOB tensorflow_contrib_util "${CMAKE_SOURCE_DIR}/tensorflow/contrib/util/*.cc")
file(GLOB tensorflow_lite_kernels "${CMAKE_SOURCE_DIR}/tensorflow/lite/kernels/*.cc")
file(GLOB tensorflow_contrib_layers_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/layers/ops/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_speech_apollo3 "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_speech/apollo3/*.cc")
file(GLOB tensorflow_lite_experimental_microfrontend_ops "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/microfrontend/ops/*.cc")
file(GLOB tensorflow_contrib_ffmpeg_default "${CMAKE_SOURCE_DIR}/tensorflow/contrib/ffmpeg/default/*.cc")
file(GLOB tensorflow_core_lib_png "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/png/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_failtest "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/failtest/*.cc")
file(GLOB tensorflow_core_profiler_internal_cpu "${CMAKE_SOURCE_DIR}/tensorflow/core/profiler/internal/cpu/*.cc")
file(GLOB tensorflow_lite_delegates_gpu "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/*.cc")
file(GLOB tensorflow_core_kernels_fuzzing "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/fuzzing/*.cc")
file(GLOB tensorflow_contrib_boosted_trees_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/boosted_trees/ops/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_speech_osx "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_speech/osx/*.cc")
file(GLOB tensorflow_core_api_def "${CMAKE_SOURCE_DIR}/tensorflow/core/api_def/*.cc")
file(GLOB tensorflow_tools_api_tests "${CMAKE_SOURCE_DIR}/tensorflow/tools/api/tests/*.cc")
file(GLOB tensorflow_cc_client "${CMAKE_SOURCE_DIR}/tensorflow/cc/client/*.cc")
file(GLOB tensorflow_core_profiler_internal_runtime "${CMAKE_SOURCE_DIR}/tensorflow/core/profiler/internal/runtime/*.cc")
file(GLOB tensorflow_lite_toco_python "${CMAKE_SOURCE_DIR}/tensorflow/lite/toco/python/*.cc")
file(GLOB tensorflow_contrib_ffmpeg "${CMAKE_SOURCE_DIR}/tensorflow/contrib/ffmpeg/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_gemmlowp_eight_bit_int_gemm "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/gemmlowp/eight_bit_int_gemm/*.cc")
file(GLOB tensorflow_contrib_ignite_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/ignite/ops/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_doc_special_examples "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/doc/special_examples/*.cc")
file(GLOB tensorflow_lite_core_api "${CMAKE_SOURCE_DIR}/tensorflow/lite/core/api/*.cc")
file(GLOB tensorflow_contrib_boosted_trees_lib_testutil "${CMAKE_SOURCE_DIR}/tensorflow/contrib/boosted_trees/lib/testutil/*.cc")
file(GLOB tensorflow_tools_mlpbtxt "${CMAKE_SOURCE_DIR}/tensorflow/tools/mlpbtxt/*.cc")
file(GLOB tensorflow_lite_testing_kernel_test "${CMAKE_SOURCE_DIR}/tensorflow/lite/testing/kernel_test/*.cc")
file(GLOB tensorflow_lite_kernels_internal "${CMAKE_SOURCE_DIR}/tensorflow/lite/kernels/internal/*.cc")
file(GLOB tensorflow_cc_profiler "${CMAKE_SOURCE_DIR}/tensorflow/cc/profiler/*.cc")
file(GLOB tensorflow_core_kernels_data_experimental_sql "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/data/experimental/sql/*.cc")
file(GLOB tensorflow_contrib_libsvm_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/libsvm/kernels/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_STL "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/btl/libs/STL/*.cc")
file(GLOB tensorflow_core_platform_s3 "${CMAKE_SOURCE_DIR}/tensorflow/core/platform/s3/*.cc")
file(GLOB tensorflow_contrib_image_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/image/ops/*.cc")
file(GLOB tensorflow_compiler_tf2tensorrt_stub "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2tensorrt/stub/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_unsupported_bench "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/unsupported/bench/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_hello_world_sparkfun_edge "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/hello_world/sparkfun_edge/*.cc")
file(GLOB tensorflow_compiler_tf2tensorrt_convert "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2tensorrt/convert/*.cc")
file(GLOB tensorflow_contrib_reduce_slice_ops_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/reduce_slice_ops/kernels/*.cc")
file(GLOB tensorflow_cc_tools "${CMAKE_SOURCE_DIR}/tensorflow/cc/tools/*.cc")
file(GLOB tensorflow_contrib_mpi_collectives_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/mpi_collectives/kernels/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_speech_disco_f746ng "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_speech/disco_f746ng/*.cc")
file(GLOB tensorflow_contrib_factorization_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/factorization/kernels/*.cc")
file(GLOB tensorflow_contrib_boosted_trees_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/boosted_trees/kernels/*.cc")
file(GLOB tensorflow_c_kernels_ops "${CMAKE_SOURCE_DIR}/tensorflow/c/kernels/ops/*.cc")
file(GLOB tensorflow_stream_executor_host "${CMAKE_SOURCE_DIR}/tensorflow/stream_executor/host/*.cc")
file(GLOB tensorflow_cc_framework "${CMAKE_SOURCE_DIR}/tensorflow/cc/framework/*.cc")
file(GLOB tensorflow_core_grappler_optimizers "${CMAKE_SOURCE_DIR}/tensorflow/core/grappler/optimizers/*.cc")
file(GLOB tensorflow_lite_tools_evaluation "${CMAKE_SOURCE_DIR}/tensorflow/lite/tools/evaluation/*.cc")
file(GLOB tensorflow_core_lib_core "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/core/*.cc")
file(GLOB tensorflow_stream_executor "${CMAKE_SOURCE_DIR}/tensorflow/stream_executor/*.cc")
file(GLOB tensorflow_stream_executor_lib "${CMAKE_SOURCE_DIR}/tensorflow/stream_executor/lib/*.cc")
file(GLOB tensorflow_core_grappler_inputs "${CMAKE_SOURCE_DIR}/tensorflow/core/grappler/inputs/*.cc")
file(GLOB tensorflow_core_grappler_optimizers_data_vectorization "${CMAKE_SOURCE_DIR}/tensorflow/core/grappler/optimizers/data/vectorization/*.cc")
file(GLOB tensorflow_lite_delegates_gpu_gl_compiler "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/gl/compiler/*.cc")
file(GLOB tensorflow_contrib_bigtable_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/bigtable/kernels/*.cc")
file(GLOB tensorflow_core_distributed_runtime_eager "${CMAKE_SOURCE_DIR}/tensorflow/core/distributed_runtime/eager/*.cc")
file(GLOB tensorflow_contrib_kinesis_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/kinesis/ops/*.cc")
file(GLOB tensorflow_lite_testing "${CMAKE_SOURCE_DIR}/tensorflow/lite/testing/*.cc")
file(GLOB tensorflow_core_ops "${CMAKE_SOURCE_DIR}/tensorflow/core/ops/*.cc")
file(GLOB tensorflow_contrib_ignite_kernels_client "${CMAKE_SOURCE_DIR}/tensorflow/contrib/ignite/kernels/client/*.cc")
file(GLOB tensorflow_compiler_mlir_lite_utils "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/lite/utils/*.cc")
file(GLOB tensorflow_contrib_tensor_forest_kernels_v4 "${CMAKE_SOURCE_DIR}/tensorflow/contrib/tensor_forest/kernels/v4/*.cc")
file(GLOB tensorflow_compiler_xla_service_interpreter "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/service/interpreter/*.cc")
file(GLOB tensorflow_core_common_runtime "${CMAKE_SOURCE_DIR}/tensorflow/core/common_runtime/*.cc")
file(GLOB tensorflow_core_platform "${CMAKE_SOURCE_DIR}/tensorflow/core/platform/*.cc")
file(GLOB tensorflow_lite_delegates_gpu_common_testing "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/common/testing/*.cc")
file(GLOB tensorflow_examples_label_image "${CMAKE_SOURCE_DIR}/tensorflow/examples/label_image/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_demos_mix_eigen_and_c "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/demos/mix_eigen_and_c/*.cc")
file(GLOB tensorflow_contrib_cmake_cmake-build-debug_CMakeFiles_3.14.3_CompilerIdCXX "${CMAKE_SOURCE_DIR}/tensorflow/contrib/cmake/cmake-build-debug/CMakeFiles/3.14.3/CompilerIdCXX/*.cc")
file(GLOB tensorflow_contrib_boosted_trees_lib_learner_common_accumulators "${CMAKE_SOURCE_DIR}/tensorflow/contrib/boosted_trees/lib/learner/common/accumulators/*.cc")
file(GLOB tensorflow_lite_tools_evaluation_tasks_imagenet_image_classification "${CMAKE_SOURCE_DIR}/tensorflow/lite/tools/evaluation/tasks/imagenet_image_classification/*.cc")
file(GLOB tensorflow_contrib_memory_stats_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/memory_stats/kernels/*.cc")
file(GLOB tensorflow_c_eager "${CMAKE_SOURCE_DIR}/tensorflow/c/eager/*.cc")
file(GLOB tensorflow_core_ops_compat "${CMAKE_SOURCE_DIR}/tensorflow/core/ops/compat/*.cc")
file(GLOB tensorflow_compiler_mlir "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_doc_examples "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/doc/examples/*.cc")
file(GLOB tensorflow_core_util_sparse "${CMAKE_SOURCE_DIR}/tensorflow/core/util/sparse/*.cc")
file(GLOB tensorflow_lite_tools_optimize "${CMAKE_SOURCE_DIR}/tensorflow/lite/tools/optimize/*.cc")
file(GLOB tensorflow_lite_experimental_kernels "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/kernels/*.cc")
file(GLOB tensorflow_compiler_tf2xla "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2xla/*.cc")
file(GLOB tensorflow_lite_experimental_micro "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/*.cc")
file(GLOB tensorflow_compiler_tf2tensorrt_kernels "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2tensorrt/kernels/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/*.cc")
file(GLOB tensorflow_compiler_tf2tensorrt_segment "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2tensorrt/segment/*.cc")
file(GLOB tensorflow_core_platform_windows "${CMAKE_SOURCE_DIR}/tensorflow/core/platform/windows/*.cc")
file(GLOB tensorflow_lite_experimental_micro_kernels_portable_optimized "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/kernels/portable_optimized/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_speech_simple_features_fixed_point "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_speech/simple_features/fixed_point/*.cc")
file(GLOB tensorflow_lite_toco_tflite "${CMAKE_SOURCE_DIR}/tensorflow/lite/toco/tflite/*.cc")
file(GLOB tensorflow_contrib_makefile_test "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/test/*.cc")
file(GLOB tensorflow_compiler_xrt "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xrt/*.cc")
file(GLOB tensorflow_contrib_hadoop_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/hadoop/kernels/*.cc")
file(GLOB tensorflow_lite_core "${CMAKE_SOURCE_DIR}/tensorflow/lite/core/*.cc")
file(GLOB tensorflow_compiler_tf2tensorrt "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2tensorrt/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_vision_apollo3evb "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_vision/apollo3evb/*.cc")
file(GLOB tensorflow_compiler_xla_service_gpu "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/service/gpu/*.cc")
file(GLOB tensorflow_core_lib_math "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/math/*.cc")
file(GLOB tensorflow_lite_experimental_micro_riscv32_mcu "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/riscv32_mcu/*.cc")
file(GLOB tensorflow_compiler_xla_service_cpu_tests "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/service/cpu/tests/*.cc")
file(GLOB tensorflow_core_util_tensor_bundle "${CMAKE_SOURCE_DIR}/tensorflow/core/util/tensor_bundle/*.cc")
file(GLOB tensorflow_lite_delegates_flex "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/flex/*.cc")
file(GLOB tensorflow_contrib_saved_model_cc_saved_model "${CMAKE_SOURCE_DIR}/tensorflow/contrib/saved_model/cc/saved_model/*.cc")
file(GLOB tensorflow_core_example "${CMAKE_SOURCE_DIR}/tensorflow/core/example/*.cc")
file(GLOB tensorflow_cc_ops "${CMAKE_SOURCE_DIR}/tensorflow/cc/ops/*.cc")
file(GLOB tensorflow_lite_experimental_micro_ecm3531 "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/ecm3531/*.cc")
file(GLOB tensorflow_core_profiler_internal_advisor "${CMAKE_SOURCE_DIR}/tensorflow/core/profiler/internal/advisor/*.cc")
file(GLOB tensorflow_compiler_xrt_kernels "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xrt/kernels/*.cc")
file(GLOB tensorflow_lite_delegates_nnapi_java_src_main_native "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/nnapi/java/src/main/native/*.cc")
file(GLOB tensorflow_compiler_jit_kernels "${CMAKE_SOURCE_DIR}/tensorflow/compiler/jit/kernels/*.cc")
file(GLOB tensorflow_c "${CMAKE_SOURCE_DIR}/tensorflow/c/*.cc")
file(GLOB tensorflow_compiler_tf2tensorrt_ops "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2tensorrt/ops/*.cc")
file(GLOB tensorflow_core_lib_histogram "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/histogram/*.cc")
file(GLOB tensorflow_tools_graph_transforms "${CMAKE_SOURCE_DIR}/tensorflow/tools/graph_transforms/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_vision "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_vision/*.cc")
file(GLOB tensorflow_compiler_xrt_tests "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xrt/tests/*.cc")
file(GLOB tensorflow_contrib_text_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/text/kernels/*.cc")
file(GLOB tensorflow_lite_python_optimize "${CMAKE_SOURCE_DIR}/tensorflow/lite/python/optimize/*.cc")
file(GLOB tensorflow_examples_wav_to_spectrogram "${CMAKE_SOURCE_DIR}/tensorflow/examples/wav_to_spectrogram/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_tensors "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/tensors/*.cc")
file(GLOB tensorflow_compiler_tf2tensorrt_plugin "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2tensorrt/plugin/*.cc")
file(GLOB tensorflow_python_lib_io "${CMAKE_SOURCE_DIR}/tensorflow/python/lib/io/*.cc")
file(GLOB tensorflow_core_lib_gtl "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/gtl/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_doc "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/doc/*.cc")
file(GLOB tensorflow_contrib_kinesis_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/kinesis/kernels/*.cc")
file(GLOB tensorflow_core_user_ops "${CMAKE_SOURCE_DIR}/tensorflow/core/user_ops/*.cc")
file(GLOB tensorflow_lite_python_testdata "${CMAKE_SOURCE_DIR}/tensorflow/lite/python/testdata/*.cc")
file(GLOB tensorflow_compiler_jit_graphcycles "${CMAKE_SOURCE_DIR}/tensorflow/compiler/jit/graphcycles/*.cc")
file(GLOB tensorflow_compiler_mlir_xla_transforms "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/xla/transforms/*.cc")
file(GLOB tensorflow_compiler_mlir_tensorflow_utils "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/tensorflow/utils/*.cc")
file(GLOB tensorflow_contrib_boosted_trees_lib_learner_common_stats "${CMAKE_SOURCE_DIR}/tensorflow/contrib/boosted_trees/lib/learner/common/stats/*.cc")
file(GLOB tensorflow_lite_python_interpreter_wrapper "${CMAKE_SOURCE_DIR}/tensorflow/lite/python/interpreter_wrapper/*.cc")
file(GLOB tensorflow_core_lib_bfloat16 "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/bfloat16/*.cc")
file(GLOB tensorflow_core_grappler_optimizers_data "${CMAKE_SOURCE_DIR}/tensorflow/core/grappler/optimizers/data/*.cc")
file(GLOB tensorflow_core_lib_monitoring "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/monitoring/*.cc")
file(GLOB tensorflow_contrib_boosted_trees_lib_models "${CMAKE_SOURCE_DIR}/tensorflow/contrib/boosted_trees/lib/models/*.cc")
file(GLOB tensorflow_core_profiler_rpc_client "${CMAKE_SOURCE_DIR}/tensorflow/core/profiler/rpc/client/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_mtl4 "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/btl/libs/mtl4/*.cc")
file(GLOB tensorflow_core_kernels_data_experimental "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/data/experimental/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_gemmlowp_test "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/gemmlowp/test/*.cc")
file(GLOB tensorflow_compiler_xla_client_lib "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/client/lib/*.cc")
file(GLOB tensorflow_core_framework "${CMAKE_SOURCE_DIR}/tensorflow/core/framework/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_scripts "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/scripts/*.cc")
file(GLOB tensorflow_lite_experimental_micro_examples_micro_speech_apollo3evb "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/examples/micro_speech/apollo3evb/*.cc")
file(GLOB tensorflow_contrib_boosted_trees_lib_learner_common_partitioners "${CMAKE_SOURCE_DIR}/tensorflow/contrib/boosted_trees/lib/learner/common/partitioners/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_tvmet "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/btl/libs/tvmet/*.cc")
file(GLOB tensorflow_core_kernels "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/*.cc")
file(GLOB tensorflow_core_platform_default "${CMAKE_SOURCE_DIR}/tensorflow/core/platform/default/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_lapack "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/lapack/*.cc")
file(GLOB tensorflow_lite_toco "${CMAKE_SOURCE_DIR}/tensorflow/lite/toco/*.cc")
file(GLOB tensorflow_python_kernel_tests "${CMAKE_SOURCE_DIR}/tensorflow/python/kernel_tests/*.cc")
file(GLOB tensorflow_lite "${CMAKE_SOURCE_DIR}/tensorflow/lite/*.cc")
file(GLOB tensorflow_core_tpu "${CMAKE_SOURCE_DIR}/tensorflow/core/tpu/*.cc")
file(GLOB tensorflow_lite_experimental_microfrontend "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/microfrontend/*.cc")
file(GLOB tensorflow_contrib_periodic_resample_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/periodic_resample/kernels/*.cc")
file(GLOB tensorflow_core_kernels_boosted_trees "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/boosted_trees/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_doc_snippets "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/doc/snippets/*.cc")
file(GLOB tensorflow_core_kernels_batching_util "${CMAKE_SOURCE_DIR}/tensorflow/core/kernels/batching_util/*.cc")
file(GLOB tensorflow_core_lib_jpeg "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/jpeg/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_ublas "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/btl/libs/ublas/*.cc")
file(GLOB tensorflow_compiler_xla_tools "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/tools/*.cc")
file(GLOB tensorflow_js_ops "${CMAKE_SOURCE_DIR}/tensorflow/js/ops/*.cc")
file(GLOB tensorflow_tools_optimization "${CMAKE_SOURCE_DIR}/tensorflow/tools/optimization/*.cc")
file(GLOB tensorflow_contrib_hvx_hvx_ops_support_checker "${CMAKE_SOURCE_DIR}/tensorflow/contrib/hvx/hvx_ops_support_checker/*.cc")
file(GLOB tensorflow_core_lib_io "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/io/*.cc")
file(GLOB tensorflow_contrib_memory_stats_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/memory_stats/ops/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_gemmlowp_standalone "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/gemmlowp/standalone/*.cc")
file(GLOB tensorflow_lite_java_src_test_native "${CMAKE_SOURCE_DIR}/tensorflow/lite/java/src/test/native/*.cc")
file(GLOB tensorflow_contrib_seq2seq_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/seq2seq/kernels/*.cc")
file(GLOB tensorflow_lite_delegates_gpu_common "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/common/*.cc")
file(GLOB tensorflow_compiler_mlir_lite "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/lite/*.cc")
file(GLOB tensorflow_contrib_fused_conv_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/fused_conv/kernels/*.cc")
file(GLOB tensorflow_compiler_xla "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/*.cc")
file(GLOB tensorflow_stream_executor_cuda "${CMAKE_SOURCE_DIR}/tensorflow/stream_executor/cuda/*.cc")
file(GLOB tensorflow_lite_experimental_writer "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/writer/*.cc")
file(GLOB tensorflow_compiler_tf2xla_kernels "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2xla/kernels/*.cc")
file(GLOB tensorflow_core_grappler_clusters "${CMAKE_SOURCE_DIR}/tensorflow/core/grappler/clusters/*.cc")
file(GLOB tensorflow_python_util "${CMAKE_SOURCE_DIR}/tensorflow/python/util/*.cc")
file(GLOB tensorflow_compiler_xla_tests "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/tests/*.cc")
file(GLOB tensorflow_core_lib_gif "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/gif/*.cc")
file(GLOB tensorflow_contrib_tensor_forest_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/tensor_forest/kernels/*.cc")
file(GLOB tensorflow_examples_multibox_detector "${CMAKE_SOURCE_DIR}/tensorflow/examples/multibox_detector/*.cc")
file(GLOB tensorflow_contrib_nearest_neighbor_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/nearest_neighbor/kernels/*.cc")
file(GLOB tensorflow_lite_delegates_gpu_gl_converters "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/gl/converters/*.cc")
file(GLOB tensorflow_lite_delegates_gpu_common_transformations "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/common/transformations/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_tensors "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/bench/btl/libs/tensors/*.cc")
file(GLOB tensorflow_compiler_xla_service_cpu "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/service/cpu/*.cc")
file(GLOB tensorflow_lite_schema_builtin_ops_header "${CMAKE_SOURCE_DIR}/tensorflow/lite/schema/builtin_ops_header/*.cc")
file(GLOB tensorflow_compiler_mlir_lite_transforms "${CMAKE_SOURCE_DIR}/tensorflow/compiler/mlir/lite/transforms/*.cc")
file(GLOB tensorflow_core_graph "${CMAKE_SOURCE_DIR}/tensorflow/core/graph/*.cc")
file(GLOB third_party_toolchains_preconfig_ubuntu16.04_clang_tools_cpp "${CMAKE_SOURCE_DIR}/third_party/toolchains/preconfig/ubuntu16.04/clang/tools/cpp/*.cc")
file(GLOB tensorflow_core_lib_strings "${CMAKE_SOURCE_DIR}/tensorflow/core/lib/strings/*.cc")
file(GLOB tensorflow_lite_experimental_micro_apollo3evb "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/apollo3evb/*.cc")
file(GLOB tensorflow_contrib_makefile_downloads_eigen_demos_opengl "${CMAKE_SOURCE_DIR}/tensorflow/contrib/makefile/downloads/eigen/demos/opengl/*.cc")
file(GLOB tensorflow_lite_toco_graph_transformations_tests "${CMAKE_SOURCE_DIR}/tensorflow/lite/toco/graph_transformations/tests/*.cc")
file(GLOB tensorflow_compiler_tf2tensorrt_utils "${CMAKE_SOURCE_DIR}/tensorflow/compiler/tf2tensorrt/utils/*.cc")
file(GLOB tensorflow_contrib_input_pipeline_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/input_pipeline/kernels/*.cc")
file(GLOB tensorflow_python_lib_core "${CMAKE_SOURCE_DIR}/tensorflow/python/lib/core/*.cc")
file(GLOB tensorflow_lite_delegates_gpu_gl_workgroups "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/gl/workgroups/*.cc")
file(GLOB tensorflow_contrib_reduce_slice_ops_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/reduce_slice_ops/ops/*.cc")
file(GLOB tensorflow_lite_java_src_main_native "${CMAKE_SOURCE_DIR}/tensorflow/lite/java/src/main/native/*.cc")
file(GLOB tensorflow_compiler_xla_service_gpu_tests "${CMAKE_SOURCE_DIR}/tensorflow/compiler/xla/service/gpu/tests/*.cc")
file(GLOB tensorflow_lite_tools "${CMAKE_SOURCE_DIR}/tensorflow/lite/tools/*.cc")
file(GLOB tensorflow_core_platform_posix "${CMAKE_SOURCE_DIR}/tensorflow/core/platform/posix/*.cc")
file(GLOB tensorflow_contrib_framework_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/framework/ops/*.cc")
file(GLOB tensorflow_contrib_mpi_collectives_ops "${CMAKE_SOURCE_DIR}/tensorflow/contrib/mpi_collectives/ops/*.cc")
file(GLOB tensorflow_lite_experimental_micro_sparkfun_edge "${CMAKE_SOURCE_DIR}/tensorflow/lite/experimental/micro/sparkfun_edge/*.cc")
file(GLOB tensorflow_contrib_resampler_kernels "${CMAKE_SOURCE_DIR}/tensorflow/contrib/resampler/kernels/*.cc")
file(GLOB tensorflow_lite_delegates_gpu_metal "${CMAKE_SOURCE_DIR}/tensorflow/lite/delegates/gpu/metal/*.cc")


add_library( # Sets the name of the library.
        tensorflow

        # Sets the library as a shared library.
        SHARED

        # Provides a relative path to your source file(s).
        ${tensorflow_contrib_tensorrt_shape_fn}
        ${tensorflow_compiler_xla_service_llvm_ir}
        ${tensorflow_lite_delegates_gpu_gl}
        ${tensorflow_lite_tools_benchmark_android_jni}
        ${tensorflow_compiler_xrt_client}
        ${tensorflow_contrib_periodic_resample_ops}
        ${tensorflow_core_grappler_utils}
        ${tensorflow_lite_experimental_ruy}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_eigen3}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_eigen2}
        ${tensorflow_lite_tools_accuracy_ilsvrc}
        ${tensorflow_contrib_makefile_downloads_eigen_demos_mandelbrot}
        ${tensorflow_core_kernels_rnn}
        ${tensorflow_core_profiler_internal}
        ${tensorflow_c_kernels}
        ${tensorflow_core_nccl}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_blitz}
        ${tensorflow_contrib_ignite_kernels_igfs}
        ${tensorflow_core_grappler}
        ${tensorflow_lite_models_smartreply}
        ${tensorflow_lite_tools_evaluation_stages}
        ${tensorflow_core_util_ctc}
        ${tensorflow_examples_speech_commands}
        ${tensorflow_contrib_boosted_trees_lib_quantiles}
        ${tensorflow_core_distributed_runtime}
        ${tensorflow_core_kernels_tensor_forest}
        ${tensorflow_lite_models_smartreply_ops}
        ${tensorflow_lite_models_smartreply_demo_app_src_main}
        ${tensorflow_lite_tools_benchmark}
        ${tensorflow_contrib_layers_kernels}
        ${tensorflow_compiler_aot_tests}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_gmm}
        ${tensorflow_lite_delegates_gpu_gl_kernels}
        ${tensorflow_stream_executor_platform_default}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_BLAS}
        ${tensorflow_stream_executor_gpu}
        ${third_party_toolchains_preconfig_centos6_gcc7_tools_cpp}
        ${tensorflow_lite_delegates_gpu_java_src_main_native}
        ${tensorflow_core_summary}
        ${tensorflow_contrib_hadoop_ops}
        ${tensorflow_lite_delegates_gpu_metal_kernels}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_perf_monitoring}
        ${tensorflow_core_lib_io_snappy}
        ${tensorflow_contrib_tensor_forest_ops}
        ${tensorflow_lite_experimental_micro_examples_micro_speech_simple_features}
        ${tensorflow_core_util_proto}
        ${tensorflow_core_lib_random}
        ${tensorflow_contrib_kafka_kernels}
        ${tensorflow_compiler_tests}
        ${tensorflow_contrib_android}
        ${tensorflow_core_profiler}
        ${tensorflow_cc_tutorials}
        ${tensorflow_contrib_makefile_downloads_eigen_blas}
        ${tensorflow_contrib_boosted_trees_lib_trees}
        ${tensorflow_core_kernels_data}
        ${tensorflow_lite_toco_tensorflow_graph_matching}
        ${tensorflow_contrib_session_bundle}
        ${tensorflow_lite_experimental_micro_examples_micro_speech}
        ${tensorflow_python_client}
        ${tensorflow_compiler_mlir_tensorflow_ir}
        ${tensorflow_contrib_bigtable_ops}
        ${tensorflow_lite_schema}
        ${tensorflow_contrib_pi_examples_label_image}
        ${tensorflow_stream_executor_rocm}
        ${tensorflow_contrib_tensor_forest_hybrid_core_ops}
        ${tensorflow_core_lib_db}
        ${tensorflow_contrib_hvx_clock_cycle_profiling}
        ${tensorflow_lite_examples_label_image}
        ${tensorflow_core_lib_wav}
        ${tensorflow_java_src_gen_cc}
        ${tensorflow_contrib_boosted_trees_lib_utils}
        ${tensorflow_compiler_mlir_lite_python}
        ${tensorflow_contrib_makefile_downloads_gemmlowp_meta}
        ${tensorflow_contrib_pi_examples_camera}
        ${tensorflow_python_grappler}
        ${tensorflow_cc_saved_model}
        ${tensorflow_contrib_tpu_profiler}
        ${tensorflow_core_util_rpc}
        ${tensorflow_core_grappler_graph_analyzer}
        ${tensorflow_core_lib_hash}
        ${tensorflow_compiler_jit}
        ${tensorflow_python_eager}
        ${tensorflow_core_platform_profile_utils}
        ${tensorflow_tools_proto_text}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_spbench}
        ${tensorflow_contrib_libsvm_ops}
        ${tensorflow_lite_experimental_micro_examples_micro_speech_CMSIS}
        ${tensorflow_compiler_xrt_ops}
        ${tensorflow_contrib_factorization_ops}
        ${tensorflow_lite_tools_accuracy}
        ${tensorflow_core_debug}
        ${tensorflow_tools_ci_build_builds_user_ops}
        ${tensorflow_core_platform_cloud}
        ${tensorflow_contrib_cloud_kernels}
        ${tensorflow_compiler_xla_service_gpu_llvm_gpu_backend}
        ${tensorflow_compiler_mlir_tensorflow_translate}
        ${tensorflow_java}
        ${tensorflow_lite_kernels_internal_reference}
        ${tensorflow_contrib_cloud_ops}
        ${tensorflow_contrib_nearest_neighbor_ops}
        ${tensorflow_cc_training}
        ${tensorflow_lite_experimental_micro_examples_micro_vision_sparkfun_edge}
        ${tensorflow_contrib_image_kernels}
        ${tensorflow_core_platform_hadoop}
        ${tensorflow_contrib_text_ops}
        ${tensorflow_contrib_input_pipeline_ops}
        ${tensorflow_compiler_tf2xla_ops}
        ${tensorflow_lite_examples_minimal}
        ${tensorflow_compiler_mlir_xla_ir}
        ${tensorflow_core_kernels_hexagon}
        ${tensorflow_contrib_makefile_downloads_eigen_test}
        ${tensorflow_java_src_test_native}
        ${tensorflow_lite_experimental_c}
        ${tensorflow_lite_tools_optimize_calibration}
        ${tensorflow_contrib_cmake_tests_cuda}
        ${tensorflow_compiler_xla_python}
        ${tensorflow_compiler_xla_client}
        ${tensorflow_core_kernels_neon}
        ${tensorflow_lite_c}
        ${tensorflow_lite_experimental_micro_mbed}
        ${tensorflow_compiler_mlir_lite_tools}
        ${tensorflow_contrib_makefile_downloads_gemmlowp_doc}
        ${tensorflow_compiler_tf2xla_lib}
        ${tensorflow_lite_experimental_micro_examples_hello_world}
        ${tensorflow_lite_profiling}
        ${tensorflow_contrib_bigtable_kernels_test_kernels}
        ${tensorflow_contrib_gdr}
        ${tensorflow_lite_tools_evaluation_stages_utils}
        ${tensorflow_lite_experimental_micro_examples_hello_world_disco_f746ng}
        ${tensorflow_core_distributed_runtime_rpc_eager}
        ${tensorflow_examples_android_jni_object_tracking}
        ${tensorflow_compiler_jit_tests}
        ${tensorflow_core_profiler_lib}
        ${tensorflow_contrib_kafka_ops}
        ${tensorflow_contrib_mpi}
        ${tensorflow_tools_benchmark}
        ${tensorflow_java_src_main_native}
        ${tensorflow_lite_experimental_micro_examples_micro_speech_simple_features_CMSIS}
        ${cmake-build-debug_CMakeFiles_3.14.3_CompilerIdCXX}
        ${tensorflow_lite_experimental_micro_examples_micro_speech_micro_features}
        ${tensorflow_compiler_xla_rpc}
        ${tensorflow_contrib_makefile_downloads_eigen_unsupported_test}
        ${tensorflow_core_grappler_costs}
        ${tensorflow_compiler_mlir_tensorflow_transforms}
        ${tensorflow_c_experimental}
        ${tensorflow_compiler_mlir_lite_ir}
        ${tensorflow_core_common_runtime_eager}
        ${tensorflow_examples_android_jni}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_blaze}
        ${tensorflow_lite_experimental_micro_bluepill}
        ${tensorflow_contrib_seq2seq_ops}
        ${tensorflow_lite_experimental_micro_kernels}
        ${tensorflow_contrib_resampler_ops}
        ${tensorflow_contrib_fused_conv_ops}
        ${tensorflow_core_kernels_boosted_trees_quantiles}
        ${tensorflow_lite_experimental_micro_chre}
        ${tensorflow_compiler_xla_service}
        ${tensorflow_lite_experimental_micro_arduino}
        ${tensorflow_contrib_mpi_collectives}
        ${tensorflow_lite_experimental_micro_examples_micro_speech_sparkfun_edge}
        ${tensorflow_lite_experimental_micro_kernels_cmsis-nn}
        ${tensorflow_core_distributed_runtime_rpc}
        ${tensorflow_examples_adding_an_op}
        ${tensorflow_cc_gradients}
        ${tensorflow_contrib_framework_kernels}
        ${tensorflow_python_framework}
        ${tensorflow_core_common_runtime_sycl}
        ${tensorflow_core_util}
        ${tensorflow_core_profiler_rpc}
        ${tensorflow_lite_delegates_nnapi}
        ${tensorflow_lite_models}
        ${tensorflow_lite_nnapi}
        ${tensorflow_lite_toco_graph_transformations}
        ${tensorflow_compiler_jit_ops}
        ${tensorflow_contrib_makefile_downloads_eigen_unsupported_doc_examples}
        ${tensorflow_lite_experimental_micro_examples_hello_world_arduino}
        ${tensorflow_core_grappler_verifiers}
        ${tensorflow_contrib_android_jni}
        ${tensorflow_lite_kernels_internal_optimized}
        ${tensorflow_contrib_verbs}
        ${tensorflow_lite_experimental_microfrontend_lib}
        ${tensorflow_core_common_runtime_gpu}
        ${tensorflow_contrib_ignite_kernels_dataset}
        ${tensorflow_compiler_aot}
        ${tensorflow_contrib_util}
        ${tensorflow_lite_kernels}
        ${tensorflow_contrib_layers_ops}
        ${tensorflow_lite_experimental_micro_examples_micro_speech_apollo3}
        ${tensorflow_lite_experimental_microfrontend_ops}
        ${tensorflow_contrib_ffmpeg_default}
        ${tensorflow_core_lib_png}
        ${tensorflow_contrib_makefile_downloads_eigen_failtest}
        ${tensorflow_core_profiler_internal_cpu}
        ${tensorflow_lite_delegates_gpu}
        ${tensorflow_core_kernels_fuzzing}
        ${tensorflow_contrib_boosted_trees_ops}
        ${tensorflow_lite_experimental_micro_examples_micro_speech_osx}
        ${tensorflow_core_api_def}
        ${tensorflow_tools_api_tests}
        ${tensorflow_cc_client}
        ${tensorflow_core_profiler_internal_runtime}
        ${tensorflow_lite_toco_python}
        ${tensorflow_contrib_ffmpeg}
        ${tensorflow_contrib_makefile_downloads_gemmlowp_eight_bit_int_gemm}
        ${tensorflow_contrib_ignite_ops}
        ${tensorflow_contrib_makefile_downloads_eigen_doc_special_examples}
        ${tensorflow_lite_core_api}
        ${tensorflow_contrib_boosted_trees_lib_testutil}
        ${tensorflow_tools_mlpbtxt}
        ${tensorflow_lite_testing_kernel_test}
        ${tensorflow_lite_kernels_internal}
        ${tensorflow_cc_profiler}
        ${tensorflow_core_kernels_data_experimental_sql}
        ${tensorflow_contrib_libsvm_kernels}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_STL}
        ${tensorflow_core_platform_s3}
        ${tensorflow_contrib_image_ops}
        ${tensorflow_compiler_tf2tensorrt_stub}
        ${tensorflow_contrib_makefile_downloads_eigen_unsupported_bench}
        ${tensorflow_lite_experimental_micro_examples_hello_world_sparkfun_edge}
        ${tensorflow_compiler_tf2tensorrt_convert}
        ${tensorflow_contrib_reduce_slice_ops_kernels}
        ${tensorflow_cc_tools}
        ${tensorflow_contrib_mpi_collectives_kernels}
        ${tensorflow_lite_experimental_micro_examples_micro_speech_disco_f746ng}
        ${tensorflow_contrib_factorization_kernels}
        ${tensorflow_contrib_boosted_trees_kernels}
        ${tensorflow_c_kernels_ops}
        ${tensorflow_stream_executor_host}
        ${tensorflow_cc_framework}
        ${tensorflow_core_grappler_optimizers}
        ${tensorflow_lite_tools_evaluation}
        ${tensorflow_core_lib_core}
        ${tensorflow_stream_executor}
        ${tensorflow_stream_executor_lib}
        ${tensorflow_core_grappler_inputs}
        ${tensorflow_core_grappler_optimizers_data_vectorization}
        ${tensorflow_lite_delegates_gpu_gl_compiler}
        ${tensorflow_contrib_bigtable_kernels}
        ${tensorflow_core_distributed_runtime_eager}
        ${tensorflow_contrib_kinesis_ops}
        ${tensorflow_lite_testing}
        ${tensorflow_core_ops}
        ${tensorflow_contrib_ignite_kernels_client}
        ${tensorflow_compiler_mlir_lite_utils}
        ${tensorflow_contrib_tensor_forest_kernels_v4}
        ${tensorflow_compiler_xla_service_interpreter}
        ${tensorflow_core_common_runtime}
        ${tensorflow_core_platform}
        ${tensorflow_lite_delegates_gpu_common_testing}
        ${tensorflow_examples_label_image}
        ${tensorflow_contrib_makefile_downloads_eigen_demos_mix_eigen_and_c}
        ${tensorflow_contrib_cmake_cmake-build-debug_CMakeFiles_3.14.3_CompilerIdCXX}
        ${tensorflow_contrib_boosted_trees_lib_learner_common_accumulators}
        ${tensorflow_lite_tools_evaluation_tasks_imagenet_image_classification}
        ${tensorflow_contrib_memory_stats_kernels}
        ${tensorflow_c_eager}
        ${tensorflow_core_ops_compat}
        ${tensorflow_compiler_mlir}
        ${tensorflow_contrib_makefile_downloads_eigen_doc_examples}
        ${tensorflow_core_util_sparse}
        ${tensorflow_lite_tools_optimize}
        ${tensorflow_lite_experimental_kernels}
        ${tensorflow_compiler_tf2xla}
        ${tensorflow_lite_experimental_micro}
        ${tensorflow_compiler_tf2tensorrt_kernels}
        ${tensorflow_contrib_makefile_downloads_eigen_bench}
        ${tensorflow_compiler_tf2tensorrt_segment}
        ${tensorflow_core_platform_windows}
        ${tensorflow_lite_experimental_micro_kernels_portable_optimized}
        ${tensorflow_lite_experimental_micro_examples_micro_speech_simple_features_fixed_point}
        ${tensorflow_lite_toco_tflite}
        ${tensorflow_contrib_makefile_test}
        ${tensorflow_compiler_xrt}
        ${tensorflow_contrib_hadoop_kernels}
        ${tensorflow_lite_core}
        ${tensorflow_compiler_tf2tensorrt}
        ${tensorflow_lite_experimental_micro_examples_micro_vision_apollo3evb}
        ${tensorflow_compiler_xla_service_gpu}
        ${tensorflow_core_lib_math}
        ${tensorflow_lite_experimental_micro_riscv32_mcu}
        ${tensorflow_compiler_xla_service_cpu_tests}
        ${tensorflow_core_util_tensor_bundle}
        ${tensorflow_lite_delegates_flex}
        ${tensorflow_contrib_saved_model_cc_saved_model}
        ${tensorflow_core_example}
        ${tensorflow_cc_ops}
        ${tensorflow_lite_experimental_micro_ecm3531}
        ${tensorflow_core_profiler_internal_advisor}
        ${tensorflow_compiler_xrt_kernels}
        ${tensorflow_lite_delegates_nnapi_java_src_main_native}
        ${tensorflow_compiler_jit_kernels}
        ${tensorflow_c}
        ${tensorflow_compiler_tf2tensorrt_ops}
        ${tensorflow_core_lib_histogram}
        ${tensorflow_tools_graph_transforms}
        ${tensorflow_lite_experimental_micro_examples_micro_vision}
        ${tensorflow_compiler_xrt_tests}
        ${tensorflow_contrib_text_kernels}
        ${tensorflow_lite_python_optimize}
        ${tensorflow_examples_wav_to_spectrogram}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_tensors}
        ${tensorflow_compiler_tf2tensorrt_plugin}
        ${tensorflow_python_lib_io}
        ${tensorflow_core_lib_gtl}
        ${tensorflow_contrib_makefile_downloads_eigen_doc}
        ${tensorflow_contrib_kinesis_kernels}
        ${tensorflow_core_user_ops}
        ${tensorflow_lite_python_testdata}
        ${tensorflow_compiler_jit_graphcycles}
        ${tensorflow_compiler_mlir_xla_transforms}
        ${tensorflow_compiler_mlir_tensorflow_utils}
        ${tensorflow_contrib_boosted_trees_lib_learner_common_stats}
        ${tensorflow_lite_python_interpreter_wrapper}
        ${tensorflow_core_lib_bfloat16}
        ${tensorflow_core_grappler_optimizers_data}
        ${tensorflow_core_lib_monitoring}
        ${tensorflow_contrib_boosted_trees_lib_models}
        ${tensorflow_core_profiler_rpc_client}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_mtl4}
        ${tensorflow_core_kernels_data_experimental}
        ${tensorflow_contrib_makefile_downloads_gemmlowp_test}
        ${tensorflow_compiler_xla_client_lib}
        ${tensorflow_core_framework}
        ${tensorflow_contrib_makefile_downloads_eigen_scripts}
        ${tensorflow_lite_experimental_micro_examples_micro_speech_apollo3evb}
        ${tensorflow_contrib_boosted_trees_lib_learner_common_partitioners}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_tvmet}
        ${tensorflow_core_kernels}
        ${tensorflow_core_platform_default}
        ${tensorflow_contrib_makefile_downloads_eigen_lapack}
        ${tensorflow_lite_toco}
        ${tensorflow_python_kernel_tests}
        ${tensorflow_lite}
        ${tensorflow_core_tpu}
        ${tensorflow_lite_experimental_microfrontend}
        ${tensorflow_contrib_periodic_resample_kernels}
        ${tensorflow_core_kernels_boosted_trees}
        ${tensorflow_contrib_makefile_downloads_eigen_doc_snippets}
        ${tensorflow_core_kernels_batching_util}
        ${tensorflow_core_lib_jpeg}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_ublas}
        ${tensorflow_compiler_xla_tools}
        ${tensorflow_js_ops}
        ${tensorflow_tools_optimization}
        ${tensorflow_contrib_hvx_hvx_ops_support_checker}
        ${tensorflow_core_lib_io}
        ${tensorflow_contrib_memory_stats_ops}
        ${tensorflow_contrib_makefile_downloads_gemmlowp_standalone}
        ${tensorflow_lite_java_src_test_native}
        ${tensorflow_contrib_seq2seq_kernels}
        ${tensorflow_lite_delegates_gpu_common}
        ${tensorflow_compiler_mlir_lite}
        ${tensorflow_contrib_fused_conv_kernels}
        ${tensorflow_compiler_xla}
        ${tensorflow_stream_executor_cuda}
        ${tensorflow_lite_experimental_writer}
        ${tensorflow_compiler_tf2xla_kernels}
        ${tensorflow_core_grappler_clusters}
        ${tensorflow_python_util}
        ${tensorflow_compiler_xla_tests}
        ${tensorflow_core_lib_gif}
        ${tensorflow_contrib_tensor_forest_kernels}
        ${tensorflow_examples_multibox_detector}
        ${tensorflow_contrib_nearest_neighbor_kernels}
        ${tensorflow_lite_delegates_gpu_gl_converters}
        ${tensorflow_lite_delegates_gpu_common_transformations}
        ${tensorflow_contrib_makefile_downloads_eigen_bench_btl_libs_tensors}
        ${tensorflow_compiler_xla_service_cpu}
        ${tensorflow_lite_schema_builtin_ops_header}
        ${tensorflow_compiler_mlir_lite_transforms}
        ${tensorflow_core_graph}
        ${third_party_toolchains_preconfig_ubuntu16.04_clang_tools_cpp}
        ${tensorflow_core_lib_strings}
        ${tensorflow_lite_experimental_micro_apollo3evb}
        ${tensorflow_contrib_makefile_downloads_eigen_demos_opengl}
        ${tensorflow_lite_toco_graph_transformations_tests}
        ${tensorflow_compiler_tf2tensorrt_utils}
        ${tensorflow_contrib_input_pipeline_kernels}
        ${tensorflow_python_lib_core}
        ${tensorflow_lite_delegates_gpu_gl_workgroups}
        ${tensorflow_contrib_reduce_slice_ops_ops}
        ${tensorflow_lite_java_src_main_native}
        ${tensorflow_compiler_xla_service_gpu_tests}
        ${tensorflow_lite_tools}
        ${tensorflow_core_platform_posix}
        ${tensorflow_contrib_framework_ops}
        ${tensorflow_contrib_mpi_collectives_ops}
        ${tensorflow_lite_experimental_micro_sparkfun_edge}
        ${tensorflow_contrib_resampler_kernels}
        ${tensorflow_lite_delegates_gpu_metal}
        )

target_link_libraries( # Specifies the target library.
        tensorflow
        )
