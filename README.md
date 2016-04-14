# ComRouting_DT_MDP
<b>BIAD Capstone:</b>
An effort to congele the low-viscosity flow of conceptual synaptic fluid into a more palpable, solidified form whose boundaries and edges, though vaguely defined and gelatinous even, will more closely resemble the completed form of a future product or service than at the onset.

<dl>What is this?
	<dt>Concept</dt>
			<dd>A web toolkit to rapidly search a large, multivariate database of notation files that represent sequential streams of musical data, in order to trigger interactive playback and transformation of stored asset arrays in real-time, while continuously adjusting the time/frequency data of the input stream to a base of pre-defined, yet flexible notation parameters.<dd>
	<dt>Feature Wishlist</dt>
		<ul>
				<li><b>Signal Processing</b>
					<i>&nbsp;Real-Time Analysis</i>
						<ol>
							<li>Fast Fourier Transform (fft)</li>
						</ol>
				</li>
				<li><b>Feature Extraction</b>
					<i>&nbsp;Data Comparison</i>
						<ol>
							<li>Routing to Tables</li>
							<li><a href="https://github.com/dfm/emcee.git" target="_blank">emcee</a> for parameter comparison and estimation.</li>
							<li><s><a href="http://msp.org/camcos/2010/5-1/p04.xhtml" target="_blank">Ensemble Samplers</a></s></li>
						</ol>
				</li>
				<li><b>Quick Data <s>Visualization</s> Access</b>
					<i>&nbsp;Extremely fast interaction with data via GUI</i>
						<ol>
						  <li><a href="https://github.com/mmckegg/json-query" target="_blank">Data Retrieval</a>
							<li><a href="http://square.github.io/crossfilter/" target="_blank">Crossfilter</a>-like access to data.</li>
						</ol>
				</li>
				<li><b>Web Audio</b>
					<i>&nbsp;Network Integration</i>
						<ol>
						  <li><a href="https://github.com/mmckegg" target="_blank">Some Examples</a>
							<li><a href="https://github.com/WebAudio/web-midi-api" target="_blank">W3C Web Audio/MIDI Integration</li>
							<li><a href="http://supercollider.github.io/" target="_blank">SuperCollider</li>
						</ol>
				</li>
		</ul>
</dl>
Quick Steps
-----------

### Required software

- Source management
  - Git for Windows (latest version)
- Build tools
  - Cmake, latest stable version
  - MinGW, version *4.82* 32-bit, the distribution shipped with Qt (QT\Tools\mingw482_32)
  - Visual Studio, VS 2013 (VS 2015 is likely to work, but untested)
- Libraries
  - Required
    - *Qt* >= 5.5.1
        Use the official download from qt.io and the online-installer. It offers
        flexibility in choosing different packages in a single go (e.g. Qt,
        MinGW and Qt Creator) and helps managing maintenance. It provides a
        file structure that accommodates different Qt flavors (Qt built with
        different toolchains), versions, and modules at the same time. We will
        be referring to that file structure throughout this text.

        *Important note*: the flavor of Qt (e.g. msvc2013_64 or mingw492_32) must
        match your toolchain as closely as possible!

        For a 64-bit VS build select msvc2013_64
        for a 32-bit MinGW build select mingw492_32
    - *libsndfile* >= 1.0.25
- Recommended
  - *fftw* >= 3.3.4
  - *readline* >= 5.0 (more recent versions can be found in MinGW distributions)
- Optional
  - *ASIO-SDK* = 2.3 (Asio support in Portaudio)
  - *DirectX SDK* v.7 for MinGW, v.9 for VS. (Direct Sound support in Portaudio)
  - *NSIS*, if you want to create an binary SC installer (add to path)
- Convenience
  - a unix line-ending friendly text editor like *Atom* or *Notepad++*
  - a extraction tool for unixy compression formats like tar and gz, e.g. *7-zip*


