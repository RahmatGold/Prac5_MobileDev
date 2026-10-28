Part A

Q1: composable body is used for ui part of project not for operations that change external state

Recomposition can also be cancelled, discarded, and restarted when Compose determines that the UI needs to be recalculated. therefore it updates ui for several times 


Q2: 

call a suspend function while the composable is in the Composition -> LaunchedEffect
launch a coroutine from a callback such as onClick ->  rememberCoroutineScope()
read the latest value inside an effect without restarting it  -> rememberUpdatedState()
register a listener and remove it afterwards -> DisposableEffect
publish Compose state to code Compose does not manage  -> SideEffect
turn Flow, LiveData or RxJava into Compose State -> produceState
recompose less often than the input changes -> derivedStateOf
turn Compose State into a Flow -> snapshotFlow

Q3:

