<svelte:head>
  <title>Widget | Velzon - Svelte Admin & Dashboard Template</title>
</svelte:head>
<script>
import {
    Container,
    Row,
    Col,
    Alert,
    Button
} from 'sveltestrap';
import BreadCrumb from '../../Components/Common/BreadCrumb.svelte';
// import TileBoxs from './TileBoxs.svelte';
// import OtherWidgets from './OtherWidgets.svelte';
// import UpcomingActivity from './UpcomingActivities.svelte';
// import ChartMapWidgets from './Chart&MapWidgets.svelte';
// import EcommerceWidgets from './EcommerceWidgets.svelte';
// import CreditCard from './CreditCard.svelte';
// import WidgetData from '../../common/data/widgets';

const handleClick = () => {
    alert('Hello world')
}
</script>

<div class="page-content">

<Container fluid>

<BreadCrumb title="Florian" pageTitle="Velzon" />

        <Row>
            <Col class="col-12">
                <Alert color="info" class="alert-label-icon label-arrow ">
                    <i class="ri-airplay-line label-icon"></i><strong> Hi friends! </strong> How are y'all doing?
                </Alert>
            </Col>
        </Row>

        <Row>
            <Col>
                <Button
                on:click={() => handleClick() }
                    color="primary"> Click me!</Button>
            </Col>
        </Row>

<!-- <TileBoxs {WidgetData} />

<OtherWidgets otherWidgets2={WidgetData.otherWidgets2} />

<UpcomingActivity

widgetsActivities={WidgetData.widgetsActivities}

widgetsTasks={WidgetData.widgetsTasks}

/>

<ChartMapWidgets

widgetsAudiences={WidgetData.widgetsAudiences}

widgetsPortfolio={WidgetData.widgetsPortfolio}

/>

<EcommerceWidgets /> 

<CreditCard /> -->

</Container>
</div>
