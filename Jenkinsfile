@Library('StudyPipelineLib')
import com.ghotfall.spl.Builder

Builder builder = new Builder()

node('master') {
    builder.preBuild()
    builder.simpleBuild(true)
}