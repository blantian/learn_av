
# FFmpeg 结构体解析


## AVFormatContext 
  ### AVFormatContext 是 FFmpeg 库中用于表示多媒体文件或流的上下文结构体。它包含了有关文件或流的所有信息，包括格式、流、元数据等。
  以下是 AVFormatContext 结构体的一些关键字段和它们的作用：
##### • av_class：用于日志记录和选项的类。 
##### • iformat：输入容器格式，仅在解复用时使用，由 avformat_open_input() 设置。 
##### • oformat：输出容器格式，仅在复用时使用，由用户设置。 
#####	• priv_data：私有数据，特定于格式。 
#####	• pb：I/O 上下文，用于读写数据。 
#####	• ctx_flags：上下文标志。 
#####	• nb_streams：流的数量。 
#####	• streams：指向所有流的指针数组。 
#####	• filename：文件名。 
#####	• start_time：流的开始时间。 
#####	• duration：流的持续时间。 
#####	• bit_rate：比特率。 
#####	• metadata：元数据字典。 
#####	• programs：指向所有程序的指针数组。 
#####	• video_codec、audio_codec、subtitle_codec：默认的编解码器。 
#####	• max_index_size、max_picture_buffer：索引和图片缓冲区的最大大小。 
#####	• start_time_realtime：实时开始时间。 
#####	• fps_probe_size：用于探测帧率的大小。 
#####	• error_recognition：错误识别级别。 
#####	• interrupt_callback：中断回调。 
#####	• debug：调试标志。 
#####	• max_interleave_delta：最大交错增量。 
#####	• strict_std_compliance：标准兼容性级别。 
#####	• event_flags：事件标志。 
#####	• max_ts_probe：最大时间戳探测。 
#####	• avoid_negative_ts：避免负时间戳。 
#####	• dump_separator：转储分隔符。 
#####	• codec_whitelist、format_whitelist：编解码器和格式白名单。 
#####	• io_repositioned：I/O 重新定位标志。 
#####	• max_analyze_duration：最大分析持续时间。 
#####	• probesize：探测大小。 
#####	• format_probesize：格式探测大小。 
#####	• codec_tag：编解码器标签。 
#####	• skip_estimate_duration_from_pts：跳过从 PTS 估计持续时间。 
#####	• max_probe_packets：最大探测包数。 
#####	• skip_initial_bytes：跳过的初始字节数。 
#####	• correct_ts_overflow：校正时间戳溢出。 
#####	• max_streams：最大流数。 
#####	• skip_alpha：跳过 alpha 通道。 
#####	• dump_format：转储格式。 
#####	• data_codec：数据编解码器。 
#####	• metadata_header_padding：元数据头部填充。 
#####	• output_ts_offset：输出时间戳偏移。 
#####	• max_picture_buffer：最大图片缓冲区。 
#####	• max_index_size：最大索引大小。 
#####	• max_picture_buffer：最大图片缓冲区。 
##### • max_index_size：最大索引大小。 
