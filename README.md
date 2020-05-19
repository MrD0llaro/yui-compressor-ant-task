YUICompressor Ant Task
------------------------

[![Build Status](https://travis-ci.org/hazendaz/yui-compressor-ant-task.svg?branch=master)](https://travis-ci.org/hazendaz/yui-compressor-ant-task)
[![Yui License](http://img.shields.io/badge/license-YUI%202-blue.svg)](https://github.com/yui/yuicompressor/blob/master/LICENSE.TXT)

Yahoo UI's great Rhino based compressor packaged as an Ant task.


Integration with a custom yiucompressor for support the new js version like Jquery 3.5.1



For build first build and deploy in your local maven repository the yuicompress 2.4.9



For use in ant remember the dependencies:




<taskdef name="yui-compressor" classname="net.noha.tools.ant.yuicompressor.tasks.YuiCompressorTask">
			<classpath refid="task.classpath" />
		</taskdef>

	<path id="task.classpath">
		<pathelement location="${yuicompressor.jar}" />
		<pathelement location="${yuicompressor-ant-task.jar}" />
		<pathelement location="${jarjar.jar}" />
		<pathelement location="${jargs.jar}" />
		<pathelement location="${rhino.jar}" />
		<pathelement location="${ant.jar}" />
		<pathelement location="${ant-launcher.jar}" />
		<pathelement location="${guava.jar}" />
		<pathelement location="${htmlcompressor.jar}" />

	</path>
  
  
  
  properties file :
 
	ant.jar                         = ${compressor.lib.dir}/ant-1.9.9.jar
	ant-launcher.jar                = ${compressor.lib.dir}/ant-launcher-1.9.9.jar
	guava.jar                       = ${compressor.lib.dir}/guava-20.0.jar
	htmlcompressor.jar              = ${compressor.lib.dir}/htmlcompressor.jar -1.6.2.jar
	rhino.jar                       = ${compressor.lib.dir}/rhino-1.6R7.jar
	jargs.jar                       = ${compressor.lib.dir}/jargs-1.0.jar
	jarjar.jar                      = ${compressor.lib.dir}/jarjar-1.4.1.jar
	yuicompressor.jar               = ${compressor.lib.dir}/yuicompressor-2.4.9.jar
	yuicompressor-ant-task.jar      = ${compressor.lib.dir}/yui-compressor-ant-task-0.7.0.jar
