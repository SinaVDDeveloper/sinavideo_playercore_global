# sinavideo_playercore
播放器内核部分，全格式版本（ffmpeg支持的）
##功能部分：
###提供类似于Google播放器三件套类似的接口【不完全兼容】
###支持软硬解
###支持hls直播
###支持m3u8点播方式拖动


##特性：
###按需解压，内核压缩包4M内，运行时按照cpu类型进行自动选择
###支持全量android CPU，包含：armv6 armv7 armv7s vfp neon mips x86 【暂时不支持64位】
###使用MediaCodec实现硬解码，避免openmax的兼容性问题
###可以支持高通、MTK、Atom等主流SoC的硬解码方案
###支持格式列表：
big-endian                no
runtime cpu detection     no
ARMv5TE enabled           yes
ARMv6 enabled             yes
ARMv6T2 enabled           yes
VFP enabled               yes
NEON enabled              yes
THUMB enabled             no
debug symbols             no
strip symbols             yes
optimize for size         no
optimizations             yes
static                    yes
shared                    no
postprocessing support    yes
new filter support        no
network support           yes
threading support         pthreads
safe bitstream reader     yes
SDL support               no
opencl enabled            no
libzvbi enabled           no
texi2html enabled         no
perl enabled              yes
pod2man enabled           yes
makeinfo enabled          yes

External libraries:
zlib

Enabled decoders:
aac			bmp			idcin
aac_latm		bmv_audio		idf
aasc			bmv_video		iff_byterun1
ac3			brender_pix		iff_ilbm
adpcm_4xm		c93			imc
adpcm_adx		cavs			indeo2
adpcm_afc		cdgraphics		indeo3
adpcm_ct		cdxl			indeo4
adpcm_dtk		cinepak			indeo5
adpcm_ea		cljr			interplay_dpcm
adpcm_ea_maxis_xa	cllc			interplay_video
adpcm_ea_r1		comfortnoise		jacosub
adpcm_ea_r2		cook			jpeg2000
adpcm_ea_r3		cpia			jpegls
adpcm_ea_xas		cscd			jv
adpcm_g722		cyuv			kgv1
adpcm_g726		dca			kmvc
adpcm_g726le		dfa			lagarith
adpcm_ima_amv		dirac			loco
adpcm_ima_apc		dnxhd			mace3
adpcm_ima_dk3		dpx			mace6
adpcm_ima_dk4		dsicinaudio		mdec
adpcm_ima_ea_eacs	dsicinvideo		metasound
adpcm_ima_ea_sead	dvbsub			microdvd
adpcm_ima_iss		dvdsub			mimic
adpcm_ima_oki		dvvideo			mjpeg
adpcm_ima_qt		dxa			mjpegb
adpcm_ima_rad		dxtory			mlp
adpcm_ima_smjpeg	eac3			mmvideo
adpcm_ima_wav		eacmv			motionpixels
adpcm_ima_ws		eamad			movtext
adpcm_ms		eatgq			mp1
adpcm_sbpro_2		eatgv			mp1float
adpcm_sbpro_3		eatqi			mp2
adpcm_sbpro_4		eightbps		mp2float
adpcm_swf		eightsvx_exp		mp3
adpcm_thp		eightsvx_fib		mp3adu
adpcm_xa		escape124		mp3adufloat
adpcm_yamaha		escape130		mp3float
aic			evrc			mp3on4
alac			exr			mp3on4float
als			ffv1			mpc7
amrnb			ffvhuff			mpc8
amrwb			ffwavesynth		mpeg1video
amv			flac			mpeg2video
anm			flashsv			mpeg4
ansi			flashsv2		mpegvideo
ape			flic			mpl2
ass			flv			msa1
asv1			fourxm			msmpeg4v1
asv2			fraps			msmpeg4v2
atrac1			frwu			msmpeg4v3
atrac3			g2m			msrle
aura			g723_1			mss1
aura2			g729			mss2
avrn			gif			msvideo1
avrp			gsm			mszh
avs			gsm_ms			mts2
avui			h261			mvc1
ayuv			h263			mvc2
bethsoftvid		h263i			mxpeg
bfi			h263p			nellymoser
bink			h264			nuv
binkaudio_dct		hevc			paf_audio
binkaudio_rdft		huffyuv			paf_video
bintext			iac			pam
pbm			realtext		v210x
pcm_alaw		rl2			v308
pcm_bluray		roq			v408
pcm_dvd			roq_dpcm		v410
pcm_f32be		rpza			vb
pcm_f32le		rv10			vble
pcm_f64be		rv20			vc1
pcm_f64le		rv30			vc1image
pcm_lxf			rv40			vcr1
pcm_mulaw		s302m			vima
pcm_s16be		sami			vmdaudio
pcm_s16be_planar	sanm			vmdvideo
pcm_s16le		sgi			vmnc
pcm_s16le_planar	sgirle			vorbis
pcm_s24be		shorten			vp3
pcm_s24daud		sipr			vp5
pcm_s24le		smackaud		vp6
pcm_s24le_planar	smacker			vp6a
pcm_s32be		smc			vp6f
pcm_s32le		smvjpeg			vp8
pcm_s32le_planar	snow			vp9
pcm_s8			sol_dpcm		vplayer
pcm_s8_planar		sonic			vqa
pcm_u16be		sp5x			wavpack
pcm_u16le		srt			webp
pcm_u24be		ssa			webvtt
pcm_u24le		subrip			wmalossless
pcm_u32be		subviewer		wmapro
pcm_u32le		subviewer1		wmav1
pcm_u8			sunrast			wmav2
pcm_zork		svq1			wmavoice
pcx			svq3			wmv1
pgm			tak			wmv2
pgmyuv			targa			wmv3
pgssub			targa_y216		wmv3image
pictor			text			wnv1
pjs			theora			ws_snd1
png			thp			xan_dpcm
ppm			tiertexseqvideo		xan_wc3
prores			tiff			xan_wc4
prores_lgpl		tmv			xbin
ptx			truehd			xbm
qcelp			truemotion1		xface
qdm2			truemotion2		xl
qdraw			truespeech		xsub
qpeg			tscc			xwd
qtrle			tscc2			y41p
r10k			tta			yop
r210			twinvq			yuv4
ra_144			txd			zero12v
ra_288			ulti			zerocodec
ralf			utvideo			zlib
rawvideo		v210			zmbv

Enabled encoders:

Enabled hwaccels:

Enabled parsers:
aac			dvbsub			mpegaudio
aac_latm		dvd_nav			mpegvideo
ac3			dvdsub			png
adx			flac			pnm
bmp			gsm			rv30
cavsvideo		h261			rv40
cook			h263			tak
dca			h264			vc1
dirac			mjpeg			vorbis
dnxhd			mlp			vp3
dpx			mpeg4video		vp8

Enabled demuxers:
aac			hevc			pcm_s8
ac3			hls			pcm_u16be
act			ico			pcm_u16le
adf			idcin			pcm_u24be
adp			idf			pcm_u24le
adx			iff			pcm_u32be
aea			ilbc			pcm_u32le
afc			image2			pcm_u8
aiff			image2pipe		pjs
amr			ingenient		pmp
anm			ipmovie			pva
apc			ircam			pvf
ape			iss			qcp
aqtitle			iv8			r3d
asf			ivf			rawvideo
ass			jacosub			realtext
ast			jv			redspark
au			latm			rl2
avi			lmlm4			rm
avr			loas			roq
avs			lvf			rpl
bethsoftvid		lxf			rsd
bfi			m4v			rso
bink			matroska		rtp
bintext			mgsts			rtsp
bit			microdvd		sami
bmv			mjpeg			sap
boa			mlp			sbg
brstm			mm			sdp
c93			mmf			segafilm
caf			mov			shorten
cavsvideo		mp3			siff
cdg			mpc			smacker
cdxl			mpc8			smjpeg
concat			mpegps			smush
data			mpegts			sol
daud			mpegtsraw		sox
dfa			mpegvideo		spdif
dirac			mpl2			srt
dnxhd			mpsub			str
dsicin			msnwc_tcp		subviewer
dts			mtv			subviewer1
dtshd			mv			swf
dv			mvi			tak
dxa			mxf			tedcaptions
ea			mxg			thp
ea_cdata		nc			tiertexseq
eac3			nistsphere		tmv
epaf			nsv			truehd
ffm			nut			tta
ffmetadata		nuv			tty
filmstrip		ogg			txd
flac			oma			vc1
flic			paf			vc1t
flv			pcm_alaw		vivo
fourxm			pcm_f32be		vmd
frm			pcm_f32le		vobsub
g722			pcm_f64be		voc
g723_1			pcm_f64le		vplayer
g729			pcm_mulaw		vqf
gif			pcm_s16be		w64
gsm			pcm_s16le		wav
gxf			pcm_s24be		wc3
h261			pcm_s24le		webvtt
h263			pcm_s32be		wsaud
h264			pcm_s32le		wsvqa
wtv			xbin			yop
wv			xmv			yuv4mpegpipe
xa			xwma

Enabled muxers:

Enabled protocols:
cache			hls			rtmpt
concat			http			rtp
crypto			httpproxy		srtp
data			md5			tcp
ffrtmphttp		mmsh			udp
file			mmst			unix
ftp			pipe
gopher			rtmp

Enabled filters:

Enabled bsfs:
aac_adtstoasc		mjpeg2jpeg		noise
chomp			mjpega_dump_header	remove_extradata
dump_extradata		mov2textsub		text2movsub
h264_mp4toannexb	mp3_header_compress
imx_dump_header		mp3_header_decompress

Enabled indevs:

Enabled outdevs:

License: nonfree and unredistributable
Creating config.mak, config.h, and doc/config.texi...
libavutil/avconfig.h is unchanged

WARNING: arm-linux-androideabi-pkg-config not found, library detection may fail.


